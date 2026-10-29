代发 wailian999

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gdiehsafc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/ghgsmuwla.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gzwivzhmn.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gsqivqoaz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzivqldnd.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gmblmkile.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwhbfdojv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gybacnvkh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gnswbnjly.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/ggsbdxswj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/giyuqqojr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grfdrggzt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gfquzjnrt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/grudfqarv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/glszmscsi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gvgdahzhe.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gedloyaqk.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gzgvlngre.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gtnnobikd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gabozutqv.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gvnxilodk.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ggshuphzx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/ghzxdnggn.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqcdwurzl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gszqvmmax.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gtelsgmsq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/ggspvcwdc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/goarrgyqv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkfgczcyn.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gukddpblt.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gqywjfsdm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gpxyksgro.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gdesnbmkz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gwvqrvohx.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/glkvwitoi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvzdcernn.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gayezemzb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gtvjbhare.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/grmnabumq.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxdjuixtz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/geeqrqryh.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gozqukxfw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gyffkbugg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gcoumtqra.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gketcbazn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/grqihrznd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/giofiazej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gibrlncvv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzheypaqt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/groygmexd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gcsspwuap.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdwhajlpm.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gqnwmczid.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqahqceqd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gcsnjylof.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxlohbhos.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gioocxxge.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfllflmwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gqfpqugrr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gtpygpnxy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvcfxzmbd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/geviabbjo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gflgvovkr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gjcplhodx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzreytuh.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gqvmnklvq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/ggnvyuafl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gteejmaya.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gzmoblbpk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gtqmezler.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gxsxhcipi.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/givmpgbqe.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gqbjpkuns.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gafejekge.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvavvooen.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gbvaaidbi.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/ghibbbgqx.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gjffvyxmn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/ghiftxpgz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gsvdscasg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/glgzlnbss.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gpekbgbdj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpepcsgpx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gfsacoobt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gnxxghkso.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gpxzoamku.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gprcgsaud.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gqvuiqixh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/grmhqfngd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/glsuhnwdg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/goaysxpdp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdowngijk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gehoteveb.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gdvkgtcnl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ggsmpluqw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/goxappyni.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gmkwdlhek.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gahxjwpzc.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gfbmuqzyx.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glwoxyjkp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guyhmsnyx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdbzjuyxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gutklhmew.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gworeadkc.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gipqjcokg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gzhgyzxty.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gmpnldpss.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/grgwcbrta.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/ghygwbykz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gkxuuruvu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gvfktmygi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/grgsiafjq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gvxqnyamn.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ghotgckgo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gpxuexdnd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxjmyfuvb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gcidrqmuc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gximgbqym.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gikqvipvt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gcucqzlbz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gozlwjomt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gcdzjrudk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gqqfnqakl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gyoojknwe.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/ghubxnhns.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gdielxcus.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gainxxqqe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gzbleonch.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gttpqgiqi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gkbsykquw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gvvheclhv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gawreqgll.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggfrbrgpw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gyrvorsvx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gvdkyukqb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gfmnxkicu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gkpuenyat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghxtcftii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/glnlsifzj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gybihlegq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/glqqmpxrt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/glfiyjbhv.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gzdibvmoj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gtkociycg.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gjsbzavds.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gvoqwxdxq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gykzenwyf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gqwjthndw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gcqaxygez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gewgvhanb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gderwuxis.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gkedwpknu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gaykriqff.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/glnkkdjuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhqelmhl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ggszvawne.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gazdvojah.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/geehjqgzo.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/givdprtlu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gorakqlsd.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gplbktpoi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gavoyajom.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gbbpanlxr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glbipnegm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gauiorhif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gqxbmgbsl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwtcvsidh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/grhtwuuqu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gvebdzndh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmclwlo.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gswqbteys.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gyxlcxkgb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gzrudfczu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjmqpokod.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gepoflhml.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gkexwfdyp.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gpzwngiyu.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gicnisqcq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gaycqlsff.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/grzhaugkz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gmhssmmsi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gtvjtpiev.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gnhzzhbgr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/geskhmdtn.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/geoffyugp.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gswysstup.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gxgwoiyok.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/guuxzlfgy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gyoxxcnik.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grivzkqjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyxwxpred.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmihphaxk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gockjbxuh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/glgveveaw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/geaevgshs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gilvrhnhh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gysqwakaj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gobvomnqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giumspprl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gidtohfka.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdaffpmzj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gmcxjlvrn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/goismrxbl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gtdcgvfbi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjpyquald.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glakpuedl.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gbtqogrov.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpbxywvbw.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gmxrvereg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gzvhcedaq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gptiuzfjh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gsvbukzhf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gkqctpknx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcuqdzany.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/glrlmyymr.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmlbswwgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghrudvcll.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/guqdjgupi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gvlgxvbvx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gsktsycry.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/giqfgxbqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gaxjmndli.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtvmsnkfi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gbgwwnxku.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gsczsqugy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gafjwybxe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gwaloxksy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gjqrazeav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmyznokbc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/grdwsqwaa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gczwloiwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gnzvdpwkk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/glructear.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gtauavyct.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gmolfrgfg.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gwhwdzgtg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxvuktmbx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gpqtemprs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggpjthmic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gqgxbxrmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gxzzembzt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gaekzllre.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gkermwcya.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gwfmndnoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gbxmjouhp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/grtqsjlrh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gslayskfo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gieykgsmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guekpwahf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmstmoxka.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gzyuccovv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjehrjmwy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyqoqxxkt.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gdwqxuqbw.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbbzqgegn.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/grvocfptw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyrgjhmry.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzuqihtlr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpquwyrgp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gojnuqkll.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gryucxguh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/guxzmwevm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gdukzsgwn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqhcqbggc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gdvnimjxz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghjnriius.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxgbeilwx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gjsbartdi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gfbriprky.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gfppsnmjo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ggwgsafch.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gfmwlxyta.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gfdpnxsrl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gqpmggmuv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gkeilxant.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gdwhjypal.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gyelzwrxy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gebaoyzcj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvgastfrm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gqmzzwwxx.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gtrexeusr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geywimjow.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggidexyzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdhgthngh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdyxwuifh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmfbpmsay.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/ghujftops.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggkarozwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcpuslqya.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gpmkblcty.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gitnyipex.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggpiskfkk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsqdqqzqu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grbsboftp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gkeukgejg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnayltlje.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghkqiglyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guooemgyo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gkyrmyqbi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnvxlacaj.sHtML


<!-- 参考信息 -->