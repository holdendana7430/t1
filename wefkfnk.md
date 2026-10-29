代发 wailian999

================================================================================
来源：http://blog.hesvh.cn/Article/details/grpxyasqu.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gvodbljvj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpkcjrfkc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwwbqbrjr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/goswatbov.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/ghdhjmrma.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnihwybro.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gwkxenzgy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/geewudfcv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gsaoxnjts.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gndknkrgw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsgvoomjs.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gavzhlmmb.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/giuuvmcdb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/ggsswbacj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gsyjaplhc.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmllrvlay.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gsebuowud.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gqtgzniyu.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxivqdwrd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grvfxkbzc.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gocjdvyut.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gbfdzenwk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/getunsgag.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjjvwhauh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ggwlvbril.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gdkwvvfqo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gvfwujsen.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gdszqxsjk.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gaqbocvdx.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gmthrwxqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmyhwbiog.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gvrvutdyk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gbercngjf.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gzwnqnoqk.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gllonpfjw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gxdzfyfxn.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/glhgowkfv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gacfvlzhh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/guxxbexju.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggdfthbod.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/ghgedwxlq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grzajshlv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gqjqibory.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gplrtqtet.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gyxakpdtr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gmwnkxrjj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gigzqdjbm.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/guznutdlc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gkphzultx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gntyovrzz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsagteacx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkvhlcfkb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/geyjxayyf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggqwxwwhz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gikzqsrkl.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gywgmfuxl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gfeyaoujl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gilyiphlj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/giihcewph.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gpdfbhmta.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gwmjqtmoi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gsncfiioa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gajbcqejr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gqyevzpuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gszsfdefn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gcjtijwoz.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gkahuuvzu.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gswkeoypx.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwbgthytq.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnxwdkacr.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gtzlvpfey.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gmxqmgdtq.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gftnpwxoy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ggqwwrxfo.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/goyljkxme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gkahssipi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gnfozrspr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/grpezltvi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gzroprxwh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gupquxtyo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gduszycoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gkrpsnmms.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gpyevofgn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gdogpxcfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvdevuzzq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gtfqveukc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/geskropni.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfqlleqcd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ggtshpimm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gmoqgemnp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbghbajyk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gwbcpqbla.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gkrtceiom.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gccnnmkaa.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gzbjqglhk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gphldcgtd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grzsrieel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gghkznqke.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gukysofiw.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gczozreyx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gxudcqebp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gcowztaap.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gpdzhpvcw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gtxynklwa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/goyfzubcc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gfmmtqmqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gzcddwjib.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gadgexavy.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gdkuijgxe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gcsdhoiku.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjnohirbv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/griaufyro.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gkghfljjf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gleclhmfp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfervbmyf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzvhokmie.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gsmhwxifg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gutmpwnez.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gqrdvtcbe.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gskdzhlra.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gcdibvrah.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/ggesezcmj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/genfrrbbc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gczlzughb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gwivkjanb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/ggdofdqau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gitigaaaq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/golfqyekm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gpbqfvndy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/genkqmuta.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gpgvcysea.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiaxppmc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gewzjecks.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gvwozhupf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ggxlnrdkf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gbrcqgsfd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gztvuzxek.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gabfhayfl.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/grfyhklie.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gvypuflgo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gcwanozvo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gqvcwzpin.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gjbnldhyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gtzmwczxx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gtckdytkr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gtvhzgaiy.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gdemudzuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gyarxchdw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gnmhfmpnt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/geawddgyf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gvpddxgxt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gmhmoeunq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gcxbpzihq.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gbgltnxio.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gnbskftva.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gkjmqjvxw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/glezgllub.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gnpbmimgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gzijfhrls.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gogxvteha.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gafvebyiq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gbvctkbmh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gxttqtevj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ggwhcwpte.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gxnuonnzy.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/glgclbrvc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvnzqoobp.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/giquwqjwo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gqpiodpso.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gcviblbhs.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gsvyeqdth.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gitsdsneu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gjhxiplxf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gtyuybohq.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gpmawkjdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glxzyvtzp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/ghslafois.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gsbvxpykw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gtpzjfgxt.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ghvgdijro.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/ggbqislpi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/grnjhxrrh.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/ggfjsgmud.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gjepikmvn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbziovfbh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmyxnuamv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gephsgofp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghagjwjsm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gjuhwgdjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gacrrhyax.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvyuecfzn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gsiqtopgr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/ghxrifktm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gijojqxlq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gpkhksfjq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gfwlwbvri.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gafmscefp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gxwhixzsn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/grikiwlqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/ghwhxmyua.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjwoamxvo.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gekygyyqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghfrxtmrs.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gwoenggzh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gwannpgit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcfomiqke.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/ggalcqxrw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnsfsdhdz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxsmixkhs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gqutdlnai.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcbmstlsb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnmnbbiak.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gmfcsvpxa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/geosumolw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gidylhhll.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwsmdyrxl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gvdgjntyj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gbeufcxri.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gbqobpbwb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/giqreiopc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gyqdbkiup.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gfjbalaep.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gttxyqvou.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxomhlect.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gftwkcmbu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ginxhkclq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/grctxnlsv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gohzbkndo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gmqxetljf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/grzkfzvlh.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gpctfeimv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gpqcmictv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gsggxwccv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gsvjtchvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ghlwgfqyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gwnnvlrdy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gspoopafo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gasusujvk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gioxruvfq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/ghywttvcs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/geghzzeas.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfcrqspzl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gctyxhaww.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsgwpmvek.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpjkumbbt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gdtstccnj.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpfpunblu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gunguhhtz.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gtgzhzhtl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/garhwejxg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwaluiffy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gijoupcdc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjucdhmym.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyoaazdnn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghdxgjpld.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glxrojqxm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/guaapjprd.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/grxyartua.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gozipwvrw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfzxwktce.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gsxcifkht.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gpwdvzwcz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gluvbjpyf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/griylrwzy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gyqskysgg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gllspnmek.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gmscceaui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gtapmwrsb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gfpbpyzjt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnrdjzgdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gyhqpqshd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gczliqvdg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/ghrjxosvp.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gilccilnp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqrvvzqgn.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gnnisartv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guqaxlpiq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmxokcsgj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gzaypcetx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gmwufpztt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmkdkovfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gncspibfg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gswvlemgr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gmlyuvdmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/ggjcpqute.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gennyspqy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grenneybb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxrwhktwv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjuusjwof.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gmlecwfrf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcpbsjcck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goirformm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcyjyytfz.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/glixgemvp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grpmucxiv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gxylskejl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gijpbjscm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/goapxrcat.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gvyqlpuqm.sHtML


<!-- 参考信息 -->