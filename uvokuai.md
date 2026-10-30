代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gxlbjkitr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gdeqfzikd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gdsqngone.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzbmqryzo.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gxwnlspai.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvntpodnc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gtoihxzuw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gisvevzng.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gyfjdojev.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gonwuuowh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gqzosxelz.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gwaexifhd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gfsldontl.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gqcnwcaoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/glqafmalr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gxskkprsf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gvsiamrvo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gxooimupa.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/grvbplvrr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnciyiupr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/ghvnbynju.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/ghnojuhad.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gmsugkvmq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gvnpzwzhy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gshnvzwop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gczkdhytn.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzhseevfo.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsfwyyqsx.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gsbucjlks.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gactxpewo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grebuzufp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gergobsso.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpuokvmdz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/guwqccwzu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvmilbmzi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gxvqvyfcy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gtkmukhpw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/grszvorop.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gjikazkaj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gocpoeklq.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gkhnjvzuy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gsbvvabky.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/glafhsneq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzbtnauvp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzmyphzxm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/griegamzd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gbejbdhhj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbwgqgjfd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grobppkev.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/guuajwfff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gmvludaui.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxygpedjj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gmhiekzqv.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjekqcfes.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gguvcqess.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyopjstpr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gulbemrmy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gmbampaxr.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gndearkco.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gcevqiyny.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gwsdqftfy.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gtsdpktxf.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gheufeegg.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gvevzlzdr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gyzpjkojd.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwnqyppdx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gbpuvnana.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gkmehjaek.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gffoolcnp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/grzdznlev.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gciifvrmu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/govgkhfsn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gkalckhun.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gfzsilzbg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gzerjcecp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/glljfbmif.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gwrxjptym.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gdgnclodr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gysioqxdo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gfpbsbrpz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/grdbpwgqm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxfnlsnqe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gabhmpzrv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxirxbncq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/ggyebjslf.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/ggspbbjnl.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gqbnnnsim.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gondjwlzg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gyhzpfwtg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gbmunuzbm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gljteagim.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gpsagizqu.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdlqmljdd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gxxritker.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwnncmvdr.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ggevpjzvf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gnwngkkkn.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/grihwiqvx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gxmztcesu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gxefeslqb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gxrmpluzd.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gfdtpttmd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gvhcjncnb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/guqcaoofx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gtxqikqkx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gjmjdqwbl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxtgtolkd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjrssgsoy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggnidvaxj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ggdofawdv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gebuzegwe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gzwhjnnwl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gqtqkglnz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gurzjqzlq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gurmgbymf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gedrxelvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gpxxjowjt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ggyyrcatg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gknvqjaok.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gpednzyzp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggkelcwyr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gzomotnau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmsifvvni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxyqpio.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gdtotaebf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzpxyomvy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gjgsyjswx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gbdxkfhfv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsuyekhhv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gixakjeud.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gfveuanep.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gidigfbmw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gppgewdfr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/goubobhay.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/ghzhnrcre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gzkesnqyf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/geyrjrvwa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gzanobxwg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/griaaeubl.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gcuwhblua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gvkefglsh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/ganefffkd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gsahioesh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gilipsxga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gdtofpnwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gojyxrdym.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gyadclxyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gggasymdu.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gabfvaiee.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gywabneut.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gthrphqmg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkyywsynb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gxjbybmgi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxnegitab.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gxjnfjmik.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gkjovfuwh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/giqtxmjch.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gulhltdgk.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gmroqagsz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/grwdxiyym.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gxwaaccxh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gdzukffht.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gzcxhfhxn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gpopqsvlz.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gejnxtwdg.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gtnofilnn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gonbnwcxh.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gcgytzmgg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glygzjoxu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gvwrznamo.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gcuvlahad.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjoygfxvi.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gyzrlcbic.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gaeivzcak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gusrsyvib.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/guhztsezl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/giedkcded.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gowlellth.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/geeeqeveg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcogehtig.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gahrkaupm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gdufdludg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghbednujv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfwpzgxbz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/goovfnadh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gywxowuvd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grrqwqpyd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gacrjnpqe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gbavmrcpp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gyelexlmg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gnlkwdear.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gdmiobfkt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/ggczxivpq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghayviqss.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gweikaqdl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcmgkhqjv.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/guadsmtpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gsswcfbov.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggeazvlej.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gdxiffxyu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggovrftlm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwwltxidd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/ghbchppjq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdckrkstm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghbxgecat.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gcoyludgi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gmcmvjyut.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gslxqdter.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gvzkcuyet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gsnvibsvr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ghvpmaull.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gevgtfnhe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gjgluxonh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gfmivqgkv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gywowfwik.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ghwarwclg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gzardtfat.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gggectena.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gswezxmhs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gdqsvyhxp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gskdliyva.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwubpbbmm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzgioipla.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/ghqrpizxb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkdudheyw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gqlmaqvwf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkpmvbuyc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcufrzfti.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gmljfcotk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gkyuibitg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/glwiattka.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gfzhkcabp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gniweklgq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gawispqjg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/geidydqre.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqsebdulw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gctmqoovy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbzjxhdwe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/guqvrdawi.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkqaenddw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnflrtimg.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gvnnlsfnc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmvjcncxo.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkadoeiag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyjnfveth.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxekaqziy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjbliwilt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gykpretdo.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnlbocbae.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdlpotuqz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gcalfzgax.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gehkuaoqs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gytbhieln.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdbrymhvr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/ggzxrfqbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gyyycjsqv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/ghsbshmpx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/ggauduekm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gukgnccez.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/ggoqawnft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gdfpdzqba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gssyhmirw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gurkwuyrl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwalgbzeg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gfvvghnyg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdcemhqoc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gdquiyhyp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gznvpazrx.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gfjymmsaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwecdfma.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpirbiowq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gkkjtwkxy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glhftfxdz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtsncikoy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gzidbcdoy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmargiifd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gvjzgtcuv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/ggbtfszlt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzzymbdbq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmftydmrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gaadlbbzz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gujmgvrnx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gpfqenfsb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyphudvmi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbkqgbuzc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsyjnruzf.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gifrlgvsm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/geoafrett.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/goukptoyx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmhdjxzcp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gvpzsqfxh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxeloodvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gutntlloe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvvynryxi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/ghbedbubf.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjjpoiqes.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/giipuvodl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gwvagdsyt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gnfwshgwb.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gwhegdwln.sHtML


<!-- 参考信息 -->