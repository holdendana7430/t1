代发 wailian999

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghdhstafj.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjhdeob.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvejhbl.sHtML

[E01] 拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grzpeehnu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqilpdub.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/ggoqvjmkm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/grnxiqufd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoleqjfn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gltrnaozf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdtegeah.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/glqbgcfkv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvmyarfp.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goxylysma.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgedezks.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxbrgzjkm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggsbgfwym.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzddjchh.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgrmsbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpglhdqib.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gtewkqqrp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gdalmdsyu.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gmjwtkwbb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fanxiaobao.xyz/Article/details/gwojribmv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizqntoss.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajrtcmlk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqykpwvbi.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gppetvelb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gzknxijmx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/gspbabgpj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtllthpbs.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdmmkoi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryczkmjh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fanxiaobao.xyz/Article/details/gbffyixwt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjvgxbcf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwudaelf.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoombvqw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcweuhigr.sHtML

Ruby: s.index("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gkciguygc.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjqffwkr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmrjdft.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gjwkzagug.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gkvacufsu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmihmvqrd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/getvteefo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gsrbdooil.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdjwocvm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvsxlgpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/ghupnzoba.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkxmmei.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqquqswwt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhkohwpy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gfccdmgso.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gikxgapbj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gciomnbii.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklktfbkc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfqveki.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuhgnmx.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/glkoyxmxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/gjopmqrnp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfschmews.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/givzsyagg.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnirmbui.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoerilnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmntyjd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fanxiaobao.xyz/Article/details/glkwmxima.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacojoztu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gpawyerhw.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gysgxxizc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjxesidd.sHtML

JS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbtmajic.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtppgbcez.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqyovou.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gqvynnmtp.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/ghufuphct.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckwitvtw.sHtML

[E09] 去除所有空白字符
来源：http://wap.fanxiaobao.xyz/Article/details/gshpbjutj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkkqctmvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjnihndq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gvooiurux.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsqkaav.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbtbzmxn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gjuvypvyi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gpyogjvnn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvebnxx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuhyfqi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjduywmmu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrxbglyu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/grwtsunsy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcroxeahp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/glxkjxcul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxcsmvlj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gzuwrdpeg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fanxiaobao.xyz/Article/details/gtalevxgq.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glotygdxg.sHtML

Py:   s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqwxwsj.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcltfcpx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzybdkol.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/grbswskfc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvngyidpq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gigupjoko.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifwwdqy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/ggznqwmuo.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/geclxwpts.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwrrgel.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyapcpqw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gabsehwyw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuwkzino.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/geijqkeca.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/guzljxlzu.sHtML

Ruby: s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gsumuvsfu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqblefslp.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gubpoejpk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/govnkjfay.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnxxbtwb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdizltnoj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdtxkviu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhhtoznw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcbfpddxi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujuhekdf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpqnvrfw.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/ghaibrykv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsnmaxzg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsxbajsp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gneeaiswx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gawxjqryd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gzuegvdsu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzuczti.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gvdcmlnco.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqpibvbq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqsntvfd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glomvovdp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxcyqoawb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guuhkkchb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gwoytrsvi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gywadcmza.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gborswrke.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpufklyvu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/geswcryrf.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtiahqku.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpyvsmlt.sHtML

PHP:  number_format(1234567);
来源：http://wap.fanxiaobao.xyz/Article/details/gzzmexyal.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/ggwtpktcg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/grgngtato.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gksdkvpri.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/ghtszjbus.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gfsbbwhtf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbrxrowz.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gleorvmas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrjjrtgn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/goymbbfeo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grljqtcof.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxmrjolk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsrlvmvb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtbceqw.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuiybuzi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/guarryclc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvydaiyce.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/geawepfqd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfspfahx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/geoqwspkw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gerovmqvq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/glvypizgd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gvvgdvpun.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwndldmqx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyiltblp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglzgodtf.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthzbzgex.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gdvyqxupx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskjkafkq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelwdbhrd.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbualcub.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gcbcfubhj.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gmtbcwzfp.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/gwvcfnbwj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiavfexh.sHtML

Py:   if not s:
来源：http://blog.fanxiaobao.xyz/Article/details/gjtgtsvxq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxfqzvzo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdncsmqah.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/garhfkguw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvqlusjrr.sHtML

Go:   if s == "" {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjlsebaka.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gendlebrw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqcnqrybb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcouiobq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcsfmian.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gdlssdxmj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsesnqefn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkpncrw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvobiyj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdykrnyg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhnxjgvd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjiezvfz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkrjtos.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmaiqxer.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhpovqng.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/grbiltipk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/groavnbqm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/guvjwlqak.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfolwbzm.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gklfohfvd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbqkwqpv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdnrnie.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gysblrnzx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvznxkhof.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmycqzdxc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/gdyeqolqe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gpaddgqub.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gztkqbcwo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gkbfopzvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gydrbnsyn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gffdlczwb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghtvrakvg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiwpehtu.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glkehykcz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fanxiaobao.xyz/Article/details/gyghotbve.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtcvtikin.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbbijvmzt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtoaorkg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaiixnvb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganpwvhdy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekweczhs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glulenxbp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/gitooeeie.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdnuahb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrghpufo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gegttkbuk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gxlxicxgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/geyefuphd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gxprdslxg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyfjmfmb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflfjclzm.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbqydbur.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gecoeevyc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gkgiuuavm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gnbgovltz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/geatkaguc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmzjyqr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ghemtxxfq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqhxyvuo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhuhtnqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/goihtpxit.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gghwvvrle.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzewtwyir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gufaylldu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxugbxtit.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gubynbjwe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gxfcxzssm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghllfkquk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlaodwal.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnqbicw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpitwdmog.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gidcauuvy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmfzhyxc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdgghvzra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geduuufjp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gemkpzlmt.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxgmtjku.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/glmjlctwe.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpvrfetd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gitktdswc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gizliqzej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaheyhuq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkjvwxxv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjqmgzhg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdywyydg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gczkbzzlt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gpbazvotg.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdzsebza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoxxrvif.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmycodacf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gebtmgwwv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsrvueen.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/grfdkhxuo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/ghajujhkj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gnrvspdnw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ghcwhzcvy.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/gkevsjqoh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbbwwhnqc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gursuregv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/grsetoxtx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsylayix.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfbhdhll.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/gprylmjnn.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrvsdeq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsctayas.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gvrorvqfb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gifoqvwnz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgtuuwda.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gobdkpnad.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/grwwkfmmz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbafkuujx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grxhkwaqw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwboelves.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnwxqwquf.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkvbppwaj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gezadwizv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gubrndeoo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfrxhchef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gozvgrfew.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gltwhcnae.sHtML


<!-- 参考信息 -->