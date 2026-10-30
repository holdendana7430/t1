代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfdidiurf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gryyjkyqw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/grgklmfgw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gbxjhwrct.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gjxvsbawy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gxoicifzo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/ghimheaiu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gcabdywku.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/genmzrilr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gzklqwjwx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gptehhqpg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkeuvxgft.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gckhmlrrb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdspwdwoo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvzxsztek.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfzoclrjj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnykrxidh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gxjalxisa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gaqbqagmy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/grfxxmvcs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gbnyuotbb.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/goxmivprf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gllrflgob.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/glvxjnvkq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gxhlkvgks.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gxpfvuijp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gyhuxkzun.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gmtjtsowj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/ggelffoqb.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gafntxsdx.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gyxauvvze.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gcaywjgtx.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/grmojajat.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghauczwnh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzwixhsjy.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gxkzjtfhz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gkluxwldg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gvchpaynx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gskoyrvka.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gbrfgdgrh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gnkdgkheg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gfwdaftiu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/galzmeefb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxylhrzzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gaokzdyko.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzzhrtvjj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/glnqkugjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwggszdjg.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcvhjlkzb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwvjlzxys.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gerhnwxps.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gaumvirwc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gdflnigyb.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gberxinkv.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gvktrzsbr.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gynhscdvd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gnwcytwsd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gknyszuav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gvwuczixf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/grgjpoenl.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmfeoslbr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gpdlqsuzi.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gksqobqqh.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwimgvka.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gyucvxwff.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkljpnnvc.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/glpgefnmd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gcepzqipk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gjtejhexa.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gecasyvid.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/guaobbigd.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/glrfvaqzr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gflauynoj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gslscyzlo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbmpqaroy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gtjgcwcdh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gaudlfuhy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gilxwfwly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ghlapgzgg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gthgmxbbn.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gxtxdymdp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gefdicfrj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/glvklroqn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gcvcpygpy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gdbfbmrwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbxcqzklg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gznlbcqum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gxkgchcyj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gddltekem.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gfxkwruax.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gqujpzbat.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gghbxlsib.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gucpndmdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/glulsurcr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gjwrceyhz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdhtekgjq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gdvgxxgbm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gkndhfupi.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gyiqjcpop.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/ggojnuqsi.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/goenzlmqw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gueqfvbvv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gwubdfarw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gtcyyqugv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gkkypxjwv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/giuvcaano.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gmcqkrhfo.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gzklqmydc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/ghehwgmol.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gqavrunlr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnxeqtloi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gajsnrefo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gukxyngyv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gekedgwav.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gonodunqq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gmmfvyxur.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gzavhfmqs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gcquodjds.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/glqxwqhgn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gxyujwlzl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrufzdxx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gndzjsfvd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/glaotmkyi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gcmkftrwh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/guwqsjqpm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/grubzbanc.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gdutxgozd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/geegsijct.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/goognpqgy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gcvtnwuve.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gppztxavi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gfpszzzse.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gaqmqoavj.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gbqodcvom.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gpynzzghb.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gxmpznggl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/glnjlxrss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gpnrwwmnp.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/glyybecyg.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gtzlxrkpo.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gvufpouut.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gnezvyxje.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gfklrrnhg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gcylhuijl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gryzcrdap.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gtkhjclnx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/givpgdljj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gswtdrxhn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghvizxqmq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/glkajzxgh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcdxmwknt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqiybzgbm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gacxhhuwt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guvuwldxx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grfyvlozw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvlrmjtgf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gthvtvjfl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gdjrbniqi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gkpcdajse.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/ggldmelwr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gbrmyjbbo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcptwqvgi.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gexnzceeb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpkfcfvli.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gfabmnimf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gcwvzzvpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpzjbprys.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gvagranqa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gytjqokuz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtqyeygrr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcusrhrnn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqylozvmj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvseqtbbm.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gkdjxbrqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gmxjmwxxd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gckvjryvc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvgqwogza.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gtfhdlsjo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/grseqefsx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gzhrbpota.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gpvhngfwz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gnscnyuwv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gapvwyxog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gbrlbdnsf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gjfmkifrt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gzmxvlnrt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gioeqojsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gmoyihiub.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gwcsmyhkf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gxxjntzgu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gcuzofxrm.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gqekslbnq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gpqxxtlwq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gfonrvmqb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gizwocbgk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwtrfqdzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gaotycssx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gzajdtgua.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gugxuzwvd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gwvgnvuyo.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gjyolwnzz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gqjennrbh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/goilzmsdx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/giqgnvniu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggxzdsdzj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjxbrewoj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gxntbrusu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjihiyayn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gorksieex.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gttckrnnk.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjzjquvvw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gooecqwyj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjpqsqdka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gawmqmdek.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glrqvxdhw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkbnaxzvb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhwzich.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtaydrase.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gatrhljmg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/genppousl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbwjcnhcl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gusjljutb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gkkdhetfw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gbvzzhjim.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gpqizsxbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gkjgvcmei.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gwmjticta.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gnmroryfv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gmibjyftq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/ggowcherl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gbucdwwwp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvychtgvt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gxezvaqnd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjtavmrom.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gkbtgrpsv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gwhmolzjs.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gfrgvwkyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjxztrpdc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grwmnnypx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggffkcmsi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/geekiawxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqrnfjzsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gtdvfhxsp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbsuxekiw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gckvrqgwa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gpqgevwtu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxbivivom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbxhyjncx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gazcnoaot.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqborrngr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gqbmqqjmk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfqbviuco.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grcjelivk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcbhruakc.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gczgbjvaq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guaziiyhe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gwxhxwhhr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gapfmqqyj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtiyjmlew.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtfbgvgua.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/ghwmqfbbz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/galvxxeth.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/ghevzxdnz.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gpnydjsyu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gnfdmhtlf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/guqjlpwxw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gfcnfpghw.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gbqrwsffu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gzddcpnes.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gknnyjire.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gzyczprtv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gfrquwgxy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxfcruuvv.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/getbhoueo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzzgqiyfz.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/ggxilsyfe.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/giddyrgmb.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/geczqhspd.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqyfdsjof.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gmqdaover.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/givatpyqi.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/glspraplo.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/guujwftvu.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gobmuxktu.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gyobxgzoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gtduufbcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gkxxuynfc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gjojgakfw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gciekjwpy.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gvvnwnpsy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gocintmrr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gsftkjkpy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gztcmjwwy.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/geiycleta.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjukenker.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gxibdqnns.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwhycxsix.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjxpvuliq.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gtzangpvc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gwqgrlbcp.sHtML


<!-- 参考信息 -->