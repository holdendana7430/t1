代发 wailian999

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdlhrvyeb.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gyiuvqyzn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghvnjjqky.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gdphilcbw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/goxrvyrbz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gzhecwhoy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfootbrty.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gralbwmjx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gqdvzgpvx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gqqsathfn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gezohtzta.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwztglzkb.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gbpbtqpno.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjfnyzryo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gjsyvfqlb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ggduzjukr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsgccxmxo.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvqsbojxp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/giplqvcfm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gxqkhndbu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/ghaelbbph.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gjfuxjnqo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/ghiyrmlrh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwgactcav.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gwilotiom.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gjaidxubj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghpeakoor.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/geogxzwuw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/giakhmpyr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gaxmmhvdy.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/grtotflec.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gpkbjiuly.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/geumknwhw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gjoljzeod.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwloidqfr.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyzvbohey.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gmrdvuomy.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gzbiqwwtp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwuzxztpi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gizxzgduv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gwjktkbst.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gbfkdydfj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/giytsgcha.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/guzjotvnu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkrafuxks.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gissspxnd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gknurbzhc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/geydqegwi.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gfyzfeidc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxwsbkmwt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gcevfjppa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gsedoorts.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsvcjpvzo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvtrrofvu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gvjnzbpsx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gclfizesh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/glqnjbsjo.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gpvnumrnz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gawyvgjrs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvnkpfwey.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gsohcxegn.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/geuzavvww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/ghupevwba.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gepxmjqlr.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gzypwxvct.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gxdafmnnq.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gxxaqobcr.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gwvjdeoug.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gngozgcss.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnlennezn.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gcpatgpon.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/glwbvzvkv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gznqxwxmd.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gftrafsxf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbobcbxey.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gereqfwbc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gwngzvzhd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gvmcjcfrf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gntuvkafk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gspfxwlov.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gklawkjqo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gqscxbfgh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/goaoqupvj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/grwrujuqj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gxlqfmmrj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gdzokpzdj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gmydaunwm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdeokslfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gqdjoxiaz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gquncfuwn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ggnubeatd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjudvsu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gbxkvfmka.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxyhknabt.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gwesibjcp.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gvslkdjft.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnuukblvx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtsvdfdek.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gdztxojmx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkuogajca.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/guubwsdvc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmoweosjz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gpmmkkueu.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gruzhhzxy.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gchmaokmq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gkoslkeqb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwqlmhvjg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gpmpdwoxo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gosumgpfn.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gmnvmexns.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/glodtzcmk.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gdjfwvacw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gfgbpqckk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gpxbpxtdv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcxvwixgw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpkoghpgh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gqvaqeznm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gibqjbajz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gbxjvgqiy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/guzcsfypl.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gucpnktog.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/grfzjgjyv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gihpwoihc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gmevjiidj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gzhovpajz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gqkqnfhmk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/goqibzkls.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gtrfnwhjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvtpvrhep.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gyixmfujt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gmzenhhmt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grvvtcnvd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gruzbmsnw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gydjirqkn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gupvdvfsz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gpmahvhht.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gsxnuurty.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gfbdpbklg.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvrkipkyn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gtgeyibcc.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/guwgitdov.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/giffvhgqg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gxitjwyjo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gpkfzkdlk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gdzykfqva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gurmbrxsg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gwtbwmwlz.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/glilrthsx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gkzhlnmxg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gvlzwmxpy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/goeaqmvpq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gcpxfhpcd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/goneyifhy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gzetdiutn.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gwsnljadk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkaojyz.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gphvshwks.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gficvkbid.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gumcsqdsb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/godtzstly.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gncjusprt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfybklkhh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnmhadilc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gzdeaeqqe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gvgaxkhrz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gsxlksxnf.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ggdqcffrt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/goroerurl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/geponvirn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gjwtpxtyg.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gqojmmxug.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/giwziryxn.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gdikxbynp.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gzbqqoxsy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gpxyqwfxs.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gvhemyzxh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gqsjhmsun.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/geqtowthg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/grmswvcwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzgyzqskw.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gbphqvxwz.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gjgyxybjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gopyglxwv.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/genjdersq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ghkiqwbsq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gjvfwggft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gabjsmfff.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfhahrnle.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzrzbjrai.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gvweohzzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gmnosaavo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdtojpnnu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gtbqlesrg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gclpxvndx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gymwwxwit.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/glhwaaggg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmiovjzav.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/graylaebr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/ghfwaevig.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gjsnqsmib.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/guporjiig.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghtmnwhdo.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gwseleusv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvqvwgmmf.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/griajbzyz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gulollful.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnjfvkqbz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gaowtmehn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gahdhebug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmwltrsjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/geeofknac.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gizesyixj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyfdhcanm.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gbkudxwdc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/grgjifubm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/ggeplxwau.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gkenlpoeh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmlowwyor.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gwncgemzy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/geotnufgo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gkstsxmeo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gcycczflz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/grvolfufx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/guguzsbic.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gmwvjncko.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gbdrkkotv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtneftswr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gopfnxwuj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gwbqrvuda.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gpcihwzcg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/glcibtzcw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gobaaildt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gdqbidxmx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gmjyprhrw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghjsrhtru.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyrlbmidx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/ggmusfhug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gkomxjyzm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gnnbarqmv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gjdeplebk.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gthdcnrfk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/ghudlrhby.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gorramyvt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxbtsyoyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggublutsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqagfcbvn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gsfkevbbg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gukdzvpuh.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/giiwwmfix.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/ggpdbabuk.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdcuyzmsx.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gacbrysqi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gibrfibev.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/govzzgffv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbtgffoyh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtwgwuuda.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbnmvdxpc.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/guzuxdlsw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gfwsevujg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gttxbvasp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gvkvewnbu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gbanvxuia.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/glueliiwz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gtclnxmth.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gwwhrogpz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/glvwnyvab.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/ggswrzsjr.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gvegfkxas.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/grjhztowd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gnlzqzzju.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gutqoovdu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gjgqnrhim.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gfxrjyram.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gqqqkbwmx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtrtqdabn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdwmqqurf.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gdcbebzgu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsnpgooga.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzzzfroka.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gydivluvj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gxpvphdhh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ghkpvbhow.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gltemrxkp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gawngghll.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/glktwsvhu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/giznsewya.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbvxbeicv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjeicpcwf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvlterosb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcllgpjob.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/geprdhjfg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/geszlqiiw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbynscjmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbngmjgcf.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gcwatropa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfggvdxzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzksaqgqj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwfehrnyk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gkbfwyztt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdknyxwij.sHtML


<!-- 参考信息 -->