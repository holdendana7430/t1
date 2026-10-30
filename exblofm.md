代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gjgymngji.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gkapkbqnh.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gognqgieo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gviiebafp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gjmzmqxyr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/ggmfeefri.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/guvjwkmys.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gcwbjupbi.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/glircfazf.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gvkvpgwsb.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/geeonvrne.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gtskxvxmd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gdengoeby.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/ghlkphtth.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/ghspzkohv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgigbhcb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gnzrypwlo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gbpetzmaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gblrzclfl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gyijaayxe.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gysgccnxq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gsbrtcbti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gtlsynfvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfunqdsxf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbapcmavk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaukmmvxn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/genyrozbk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/getswwqtn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/guffvcfkh.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gwolonvaj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gnzawhioa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gemcvxksm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/ggokdjasi.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmxhsuakx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ghafbkwmn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gqqbdqneu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gnvrmthzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gtvsyxtbp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gxsqheiis.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gyaufcrkk.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gzmhfqtvy.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/glahpyjdb.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gogjmejwe.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gmahglzed.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gziwycxau.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmclmeofh.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gjlougfti.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gnzgqakzq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gdeokwujy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gbfotuxyi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ghnfyfpaq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/ggiwikihd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gnsbujiql.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gofyphcmk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gssbcrtha.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/ggtkeiswv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gygilwddf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxpmntoeq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gsshraigj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnizklkzy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gdmjwthiw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gsmnzjxcm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gjsghhloa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gqlridhdw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gwelssyhk.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsprxriep.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gzeqvgvuq.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gpvqwahdh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/giksxliiz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gamgwnszv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/giasimxxi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gdklpywvu.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gnqbaxhjj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqxetjvfa.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gfqrorzyu.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/glblapheu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gejtdcerp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/guqernyuk.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gmyrdmqqt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gxbgeygxt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gfcspewbx.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gplktczps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/ggvzjonsj.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gmqftalap.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gklfxwfiu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhcznbq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggtngjumy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grpaqsssl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/glgjevtpv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gzgffpzse.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gzxmqfbhc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gbhahovpi.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gfzpbbpoj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gyejbuhpp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gqrvpjgjh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/ghptbhtya.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/grurgclyk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/ggpjnfjfk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gnlasykis.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gdnvxjlxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gzqhmzmvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gtfccvubb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhtbsoym.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gkfmewakl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gqhuzdcqc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwbebwf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gvykxejfw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxwoaxa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gwxycxpiz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gishhjuwn.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gealtjcty.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gfjwwgsry.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/glvvzcnmh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gttnfytgu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gnvrybzhu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/grkukndef.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gykpmppnh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gfjyldokh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gnqayhyjq.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gcfriqueo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ggxplwkls.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gtdhlhmjw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gvnndbwok.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ghhleitie.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gzafiffjw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gbpsvikhg.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqqdpdjss.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/ghnppnyvk.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gpzfgzisk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gzmqpnnvk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gjvnxwiio.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzzueyyhb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/guirvzgne.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtsvquums.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfvowoivk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gloxqjxqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gxfdefdmv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gokdzvfhu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/grmuqvtkw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmvbtkful.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gjujkzdeg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gdjmxmhhy.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjgcivwui.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gclpltqud.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/ghdfdaatf.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gonncsgko.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gnkurydpb.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gergdphmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gyzkpmfuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gxooavbjs.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/geusgxfhm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gvofqhbye.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gsenawiqd.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gednqrhry.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvprwpibz.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gmrmrfeqd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gclvjfguy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbbaneuzy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gooykvrot.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvhnmnyzj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfjjlqtzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/ghlesutlc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghjqdklzz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfplhivhl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gixaqduqi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gabuekode.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzslfnfxj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gjarmamuu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/glmwduhzi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gslbvjcfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gpfsucnus.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gwyojvlet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gckezpdcr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gidzxhxyd.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gamarxhpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/govelkjay.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gpdxgikxs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gzidaqnkn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxxfnibcw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gllpgtqkb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwojkxxul.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfqnniyfw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gotaaoldv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfhxjkhap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkkwqrphz.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gdlccgbls.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gyytbalhz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gtachzyuw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ghoiqomno.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ggzghohgx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gokdyoesb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcptxvi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gzumpxqmh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gujjortze.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gxfqillhz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gojlbgovs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gomjmlioj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gnxbzefwx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gemhomeiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfscopcld.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/glzfhjdeo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gwkkdkyhn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gjjjyxtor.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gnjhdunsz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggrhmrkol.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gmpjnzcon.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gybsecbru.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ggonnmhma.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gauodsogo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjgninvgt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gjbgiohic.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gjmruvgce.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/guxvptxwq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gpsmadryp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gicrsnuyg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsykcxlwq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkufcqnwl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbbndcyjp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gpkrafsfg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvpihnjcp.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbdnhrcuw.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gsshomjht.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gchzvsopj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gziabmnci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gimwzjygw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghudgeuwk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggjfeozot.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqwbxyfpd.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gznhamuuv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guwggmgfp.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/ghmazfcab.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gpxydtudu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmskpjubk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gmzttbajq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gwlzfjdya.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gpwdtoyan.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/ghctzfdqm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/giwvcqimx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/ggwqllncn.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gmsqdtmzc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gvizlqixa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gzmqwinuw.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/grfndeysp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmawuiqcp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxhlbudun.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/grqrpuqse.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/goxxajetq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gmybuqwoi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gsrxcmrbr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxdpmfmcs.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkabbuwat.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gheroasor.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gzvhywbry.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gojompvjv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gigtypslu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjqrleefu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/guntjaikd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gtwjzkvez.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmxaffrsp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/genfrvkfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/graihsdnn.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpgpmwzov.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gvpruyxhw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkpkjsvlp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gawchnwlz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzzkrftnw.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gegknrlqz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gysklsyra.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjjiajaye.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glpaxokak.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfqozfeop.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtjeanxas.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gptkdbckg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmksdsrhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gmdxswpak.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gshqpbyxl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gvmkzfjvj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gkfnwowqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gmwvvadnx.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/glvdkcadj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gdpemdyer.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/govrufjcb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxipfrclv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gfodomlve.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdooennyn.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gnviepclp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfoydarom.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gfyzotqxt.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gfwzrihao.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gfftvosbq.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghqrolfof.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gzbgolynp.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gzshzsgfc.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghcduvbet.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gpeogontr.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gaxakvjih.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtmbfhwtw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/glqhvezec.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gpknesths.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ghcmuabqg.sHtML


<!-- 参考信息 -->