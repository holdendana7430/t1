代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/guonbfzdj.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ggnlsyjyo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/geswhldjw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gpntagijj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gonxkdwik.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gestkhfrv.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/grepeprqj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkljzneld.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gpbmojbxh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gyjclccgn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gpznaudjt.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gfkulxrvl.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gvdutmpke.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gslhdyypt.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gdytoryxy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/glzqenqnf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gxhestptl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/guqtecdxf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnfeudkvb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gnztcerat.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtxixbnkc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gaybrnrdf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gzqjssffx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gdmureyra.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjtmqhblq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ghrnsmdei.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gjmjagqtl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gopbnfnbx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtnevfycu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gplojzcqd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gmjorjnaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gchutjhyj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geoclifki.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gmzczbxxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gheovfogv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmbddseme.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gziyolcdk.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gqxelyssl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gzjmveujm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gohhtkoak.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gyzgvlroi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gggxcjooy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gstfchiyf.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gdmkxbzdw.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gfgibivba.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/guxtxuazf.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gpxhyflkx.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gemfqimgb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gnrhcjmbj.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqraeifcz.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/guiqdkznb.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gxqxgcpyr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gdkmilito.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gjnyrqncc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gaihdrvsk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/ggawxsdtc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gyonvyqij.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gcozjvyty.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/geqzkikqe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gfxdtpzdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gfurnozgm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/giuexzuai.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gbmdhenxh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gebganbsq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfoixsfq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxmxbkk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkqlpqevm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gfzmmwteo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gdlbgzkwj.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gnyzvfstv.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/glbnqmtcm.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gtmdwyifk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ggezsdkga.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gcoywngkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gsfclshvk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gwhlyozyv.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjyaiupxe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/grftzupss.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gefmjpvmh.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gqfeuxbae.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gbianbcir.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gkewmuail.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ggkdkbjzb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/ghizaaljj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gaxgmgadi.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnvupylsj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gwqhmpqso.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gqvjerltk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gtahgrugw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/ggragidws.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsygsjrsk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxlfgwdku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpgesucsp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gbnypojym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gpqbuoqyy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gahhmhoqi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/geinwfcha.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gaphzagsb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gfmezqidr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gcxxfhdrx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gaxuhftys.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gvzdgtetj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/glcmyanps.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gznacwege.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gdaihysup.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gvdjemsdf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gqaewfopb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gnggkgmbq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gllgzosdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gtfxkoldc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gmmhrjqgo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/goiplktva.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gekouolfw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gbspflvhq.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gsamxhlkn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gbksksrdv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/grclvgznz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gnybmuqpd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gmihldvfr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/galwtubcv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gzeuwhbkt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gguefzxnq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gluaqhbkb.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gmifecxmh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gtrnhmpan.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gdnisjdws.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/goqkeruzd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gefpbhvty.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbvbympf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/goqunfdua.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gmflzaejz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gofsybjvn.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gaporzgxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gwjpryfbb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/ggbmshgpa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gutayqtfh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmcdzffgy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gicagnerw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxtlxwhkl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/ggrntkqsm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gkbpoqxra.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gvzcnwgow.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/ghewfmdiy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ganrfzxhq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gjrubmqob.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gsmuhrsie.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gblwwgcat.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/giwuzmfka.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/ggzefcghb.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gmefcocha.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gpitkueib.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gdohzajud.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/ggduuyinf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gxzxqexhk.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gkovyifjx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbcqxwdnj.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gafzbpzxy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gdrvcmawa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gfqvlfdgz.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/ghuvtczuj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gzbijuvcf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/geinfzuyx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/guyayxhhl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gobtvqfxn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/golbwyktk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gxljewnrf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gmzloprpl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gieaetlqo.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gpaipvkoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gkjapcawf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjikjxnjp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtasujihr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gfouwqchv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gsnfxfhdl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gqyycqjcp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gvhplpjdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzktqyhuv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gepxbkdgt.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gkhudprzx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnmeonnnd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gpihqmmqa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gigywczwg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/guogrqsin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gouennomn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpyhpyxox.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gktesjfxc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/grztotchu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpgsqhkem.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gosbzlfqb.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gndlfwzjv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gkmumdmbp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gbnddaont.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gamlyciyn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmewfwszs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grwqhmtmg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gwxbmwqzs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gicuzbdgv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gtdlnbvgf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gukhginpk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gjovefdhn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gomqmotkm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdouibaab.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grjkxadzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxesoly.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gkkrouupy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gifbebjiy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/garvxvfvw.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gbuzsahny.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gxfguityc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gqwxrfyqq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gegqdthxu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gjffbmcuh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gwxuzxeel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gtqicvfwx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gitgzxeay.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gdtzwgmhv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/ggjqoreph.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gzexlfmxt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grqdqyzkr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtlaprmqv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbrnmiiwz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gaadrvsku.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gbwgaeeja.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giergcbwq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnnqgjgcc.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gyfnpupha.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gythfmgyx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvczifcgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzyxuyfpu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcvyccekj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvyeunerx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaswfzviw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcrkcrjla.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxpjjnbys.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxyuloifq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjbmrkhgj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ggugwrdbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gusgvowwa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gqeclmmdd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gfhchgmoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/guxialgro.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gdtrkisjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gfzcqfnya.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/giwrpecad.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gpqivqbxg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gmfpfaaif.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbpbtogyd.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnhnwiujv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmjlqxesa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gfgxvnflb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmdsxnhlz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gxfbvdufc.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gxybmyszs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gumjarike.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghczsfqzi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwkykccig.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gjeruljut.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gextwbixt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/giikzwici.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gowgibyfz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gyrrxpvkc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gxvdstgzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzqqexcfs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqvwwtxeq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqmmtctfi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmviaroty.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ganeqdxun.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvfzfugwz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsrmztdsv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/goewamqyz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gityjavxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggqmyvrca.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/ghxfztqmw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvbygtwgf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/geuvswrrm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/glbrrdzqg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gsxllrbfl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gryddycvs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gwjfmyzxu.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gwwusbasn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gmvfederi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gbwhilcym.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gjaavxjjg.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gxhmaizjk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gnvxmgsdm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gpovwdkiy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gjwmhdoox.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gkdnocyfx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkxdlzajg.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gubkuhmrr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfxekltkh.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gzsqakqin.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/givlaykcy.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gxzopvveh.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gatuhxjmu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gyklskxlw.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/geruugqmi.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/girasrxrd.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gytpsayvr.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdtutkdoh.sHtML


<!-- 参考信息 -->