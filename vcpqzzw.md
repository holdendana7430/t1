代发 wailian999

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gwyqrkzqy.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/grbhxmghs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/glndghqyr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gmakvftqr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gixrhbqdw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbxaccuho.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gsfmkxxop.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gsfpsgpxj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gnueuudrn.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gyirbaxvz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/ggkibyrdz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqveqfawe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/grgxnhmsd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gevkpeqrr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/geklbsjwx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gebimoqjq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gpsipucch.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/ghpcgvehl.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gcwzjsjth.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gxttvtrqz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gjirqkodo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gyqvtaihx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/grvfokjxv.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gapwssdhz.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gomuesnbi.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gckhlhyqx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ghmxpqwkt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gnyorpuwz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gqxfewxvw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gujmmdiht.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gdnksfwbb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gkqyfcddi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gdsvdgile.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/glbkzzfsh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/geddflcct.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gldbavxfx.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/ghlzwtust.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gualjbwpc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/ggixijuqg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gwscmpbxy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gmsntggas.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvlvddagp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/grmgzqdyf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfdayseps.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/grbaejdea.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gidvvnxnr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gmvawmoyj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gezpdtcdn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gnzjnddnh.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gtxrlbdxg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gfttehlvy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gdsdmibwe.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gcprbetou.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/goshbvcor.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gesoogtnu.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gqzobdqqr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gmlouizvu.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/goxxjcwjs.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdrckygvw.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghshlvuwq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gvttwvrwh.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gehpaucvd.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gnsprszjy.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gmzelnyyd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gpxsdmdlx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gidbpkxcc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpckthrgi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gzvbjidjk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gbkfvfytx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gtyuxfohn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gvxtcmsgs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gldfczltp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gakoobkjq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guaonwfhz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gpzfthdur.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gkalgkunf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gdvzxqgjk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gextrdbrk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcbtjsmor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gsshqevuk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gulkdtnrd.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gqiknkitc.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gggdruvbn.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gqbgpfgwt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gippofdxj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkulgtrcn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gkplewtun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gkwwtesac.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gxwqkcqui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gwwgzigbb.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gicfdmada.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gthrktxcb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gnhpqvppk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gpnyuoqgz.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkjocnklc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gzptpvciz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/giwvyijkv.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gcfusnxhd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/ghywdisfy.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ghigleqdn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/ghxiynqds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gtzjjwowi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gzdbxwmwm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gbmfnbkli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gakyeakpk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gimgyhbdm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gcwmysrdv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/grgyunzus.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gjhqhrplf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gqqjaoign.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gvegkrqvu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gkowroulc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gjexjnvym.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ghyyebcoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gbkrkcqqy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gaubqlodv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gyaaclxnq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gaqegpolx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/goqnkiurr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/grdwqhcaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/ghwivehmn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gmsybcwwa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gowkprstj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gumfoomvn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gitysnxyg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/grlgsesxb.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gtxrngtzt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gruifanlz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gxjxjzylu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gbhnholpc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gmszuokax.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gplgbokyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gwzrgutfp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gkdixzwmw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gbmwnswju.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzwaybdyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gybmyzjci.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gwklbmffa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gdaluhgit.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gwmjuwucu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gnjebhgkr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwhswphxq.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gttqrsufs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gktjflwdu.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gcdfjvayk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gojapgqvm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gbsmpxsyt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ghwhjfvsb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gyaafsevv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gygfzckil.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gaobogeis.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gxxaogadw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gzxzobatq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gpybmtizu.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/ghxrrzfzb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gjwgkuwll.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gfridblaj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gzkrmkgis.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gmiqmlciv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gvtzzjzcu.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/glihqwcbi.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gazwcspyo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gdxlktawy.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gsxhmizni.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gunjxzboq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gqkecksfd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gxeufrpbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gfesgjtct.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gsttuyqrm.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/ghizykinw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gkfldqqda.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gbmcvcwcj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gpkomhbds.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbekqgzfk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gywvcdtpj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvovttoga.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfyhvsswd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gjasifgzt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gihexveij.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gntvvzhya.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/goncdrinr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gwtwuclem.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gseavipwp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkufgbfbe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gfjabqfhk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gipghwqyd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gbxjtxjrf.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gksxdtmpr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gallrzldo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjjvsflma.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gjcewgqox.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdzfdrpmh.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gsnfirwzc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gnzwcscch.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcwxpgkof.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gulkdejsb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggooronzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gapdxznyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gznwlepbb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmiqktgjf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqtjjssyq.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gbqhzqtpc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gxmyeuhua.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gocyfdrmk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gcyxsfemc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/glubheelm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gvgtvvsgq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gcserxrev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gowserinq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gefkagvyb.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gbdoyilgw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gtmbhhyrs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxhitcsbj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkwfvhr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/grvxxqxix.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gxhsslkgv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gjwcqnxqt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gvthtbifk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gljnkinux.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gbzohxlel.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/giswmgsbg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gfogdqcrc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvmhibxlz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsyykzedp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gwnbcvtlq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gsdsiacxt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gsbrevnbf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gzyalgszy.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gjjfiydtm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gocvhebms.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/glrigcvuw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyhogwjzc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbfeiemcb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gfnlvpoyu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/ghwgpdrkb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghknfcjcj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/grghmawvm.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gwdhtjvgq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggddjbxie.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxnmpqitv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaduhagfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmhwkbnwq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcvrsbnaj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpyjthjdu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtjqfxbat.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grxhqkchf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gfcswqpdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gprghjigi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gsgkyrbkq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gijdnbrng.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gumuokfuv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/glecwetjx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gwsryxmnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbxtbvhty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gplfhkyjx.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gaavbkwgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gfvcjxgco.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gtzxeegdp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gbatyhjbq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcfigdier.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gwuvyuygc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/geqmfnrjg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/ghyjpzqxp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/guqirbwwv.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gaoebmovl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gntcgcuvm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfykrqdvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdanqkytw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gyityvfzf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gncgcvrne.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gxrhtyiym.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcnbgpzvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gqpvctlee.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gflesrnrr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gvqzosgvl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glzcjpxma.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grlyugtth.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyhrymgix.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gigmpfvzb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqnqmzmjc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqmnpeynl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gymvurkup.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gvwkmuhwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ghjpufjat.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gnsmzxhib.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggnvdnsbd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghjqauyea.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gielbrewp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gidvtighz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggmjnidof.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gneagwaiw.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/grfysnbxe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gjxetnobo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gimuizvfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gwxuidcxx.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/greawzimq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gioqyllne.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gwjbwhzgo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gpooxoves.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gwlmcyvzy.sHtML


<!-- 参考信息 -->