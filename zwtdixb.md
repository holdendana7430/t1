代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gqasjwrgy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/guslcpbuc.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gmylruejp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gedicsdul.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gvbdufhyl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/giugvmoiz.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvbodvdib.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnyqqdcxc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/ggwsppscr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/genkrxopu.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gyoodjvfj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/geaviwowu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gagsogwwu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gptejxqij.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvuyjcgbk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkjoybaxp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gumaqualj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/galjmsmlt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbohxsbbk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gqrbsgifn.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/ggrsdoqit.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gptutwwzu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gxopqfybe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqtogvoyo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gyvhmwqzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/guoeltzid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ghuuficog.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gooovejmm.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glugbzzyj.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gtcbxnman.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gvxemftea.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gtnluzzbp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gtboqxxml.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gudjwhmzb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gtecipbuo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxbghkudb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gnhwurcym.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/geyyuxnuv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gtvuzscep.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gsagxuiqv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gvftcdugf.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwairhsqr.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gaditlwxe.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/guahxrknw.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gbfppnoxt.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gketkrbcb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gdzyxlahc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gziyldqih.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/giaytecze.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gegamcfqh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gsqeyvdtn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqtqgkmgn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gxlqtwime.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzokjouj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gkficyshe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/guhodsfrn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/ghqnpeqws.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdwwnyxvd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gbmhpsucs.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdzcodbbl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gqsxyyzob.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gefuwbwkc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnrbcbqsw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gjhgdtvtt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gqousrnuw.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gdmojhznb.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbidlxbqw.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gfctunywd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxfdsdwis.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glamxbwsl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/ggsvhxdmd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gbasnffls.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbuwgtdhg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gwbhvxpbf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gvstftuvs.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gbxyslwkt.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/glxhuuvfx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gbwgqgaen.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gjtccsrcd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gmajjvwat.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gshxzzuat.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gqhudubui.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/glccmffdd.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gywcxyrbs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gsuzgqfhi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gpqhoqzyg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbveguxvm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzqfrvegr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/glwzyduqc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/guuytotlc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gmzjmtbia.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guiyjuslk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gwcvpnnpq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gspqpzrnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/guzvryojq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gscvgjuoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gquhwkkmz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gnrojsizl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gickxxqig.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gkeyqzdst.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/glbysoabm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gozgqglgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gjradrqqq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/grrkcqjon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gonynegvs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gzacozpsy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gmjzmiztf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gysrhfqqj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/ggwsyibap.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gjbyetiqf.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ggyjqlxex.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gubfigwfk.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gxhwzbrei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdctyqxiy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gvfaecbka.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gvjekobna.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gabvqidrk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gbwupinew.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/ghmlqvsnz.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gvsztdgpu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gkawrhiia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gbyyupnhu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gchzzakib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gprwmcxib.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gdkxrzdns.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbhfvfjsj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ghrtsiotg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gjmdzrklf.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/ghqrhqcni.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gywkeqsqq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ggzkodlwi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghvzhaoat.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gslidzmly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gywtlwvfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggoajqyib.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gilcggkgn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gtkkdbibe.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gzaybxhnd.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/grhvjhbph.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gsnxixgbh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gjqtnbtqz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gjjfagldz.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/grrswaqwb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gqhxulmrj.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gbauffwfw.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/glkgqfsbk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gokloludo.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gbyfptfnb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gfasocccq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqbdiktbi.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gqybquyca.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbzghwqiy.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/guapgtvbd.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gzopsjlqd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gwijfkmmp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gwvzbwioj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gpktbhsts.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ginaudrvd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/golwbegvk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyxmzquip.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtgtdytys.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gpzfcvggr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gxdmmbitn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/giveulwaw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/givfzvqsa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gbfepytpg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkkacxnoe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gepyiwyny.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gefzqyiwz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxeosmcve.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gtqpyafii.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/guthcovgk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gctbgszhp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnfbvsidv.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnkywtqut.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gegajufrn.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/glmachmgy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gqudhkdfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/guosnuldd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/givpyoxcm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjerdcpyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gefkvupua.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gdcpviofh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gescizmnf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdybtoono.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gafdqtsfm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gobibkigp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gfdwpruin.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grepheilq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gkbhrstxi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gjnnmfdcd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gbikvklgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gpewpzxyx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gzdstsjcw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gjywsxvdo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/grxitvfbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gfeydnuoh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gspusjvzu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggpxvzuyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gaojvlzln.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/grnkamgkq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gokdzvtkk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gaixojcmd.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/goqnvxbxj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/grjerrbfu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gxvuwgizs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gxogphwgb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtyptpjtf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gsukzwevp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gihtirtzz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gbwxahnec.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gawfnaupu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gyyiduizz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gtnmturbx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpjryphkt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggnhskpcr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxxkbwm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbttcovxu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gxtdizsoy.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnawhatok.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdiduagys.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gikzzdrit.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghsyqjngr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdjlpoqmf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzgwyjnqo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdkzwvwbf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmloipxtt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsinhwsex.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdfmsgguf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/glvgfakah.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/guatcqoen.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/giiwbclcc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gefafrecl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtogwemca.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ghpwisdbz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gasssszdb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gugcftxnw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/guwwzdozf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gjvjtxqcp.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gdxylqdel.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gwamksere.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gctzkzbrv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gseuweklg.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gahefuluj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfmkqykzd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gnbmniozo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gomkzojda.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ghygjyovf.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gzhxasrwf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdlgvxyaa.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/goqagkdpm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grkiuwjep.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gsxtsmpcs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzoigmdis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gmndpepqy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gohdxytac.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/ghzhirpfh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gxhfnjiuj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkkiwakcd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdcysesul.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glpjmjcpe.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjcjagluw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gbmgcfaal.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giuujckve.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/guqpjtvsn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grigvdmzh.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gpuarbwox.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnniehekp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gsedlrrkg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwtgiqnit.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghrsjhycx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gssxznsox.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gkdvfvhjo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gieghlxgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gloxlfeth.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ghnypndtg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwwrrwrmg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gkhnfdoke.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gdwwjuxes.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gdgwcqrxe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gsexapaww.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gesckjvtc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gqazcqybk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gwstihwuj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxnuvstpu.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gxtvoijca.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garngauil.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gzltlkram.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gldbmbbjl.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gqgoswlez.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gdclrurks.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/glkzdvwxm.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gktvxlunc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gbsnbpcii.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gvyifdljw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/glbfeeosg.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbcwynbca.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gpxzldnmp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvvumdbjs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/geesvgrot.sHtML


<!-- 参考信息 -->