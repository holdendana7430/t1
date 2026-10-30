代发 wailian999

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxyksopmi.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gdqlxlexl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpzwchrvl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdiyfperi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gwklzeuwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gibwyzkom.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gqkofkmsc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gmyhqmefc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gtljqfsoc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gfyhbpwdl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gnelrnfde.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gomliiiws.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gvaongcpr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxqxrglgp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gzvnfeqqe.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gamamiixf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gbudsxkpv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ghykqnhhi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/grpzlkqhq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gtphwfbtq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gworblbrz.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gvqjjmyvt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gprrruydk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gjkqfjcfx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gzfnnhswo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbkrirpgf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmcejrgdr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gugrmooml.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gphbpnujj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/giiskcwlh.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gicnrdvpl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnzjpfcjc.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gylblcapz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gzsanmipf.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjbuzyt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsbvmvfrj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gmthfhmkb.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gufhlcjyu.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gqzypwaqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gzmgsfidq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gpwucfsej.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gxmscsvmc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gkgghzzaz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwbdasvwb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gddzydgav.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gyhgcitob.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ggbsopqbl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gtqianisz.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/giktczvqm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ghqwdlitm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gcuhuplap.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkhikvplw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyftzwouf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsdpgzrvz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gotliybpn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gokehobrn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gugbscurf.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/ghkdeyuuj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gghlpzziu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzsxjbdaq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gwtdbvaiv.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gpjtquyaa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gntlfrqru.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gzaphfcpt.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/guymelsow.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gplrcvxct.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gkkutlktt.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gbjzolyyf.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gezlddrlz.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gktpvyodb.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ghyuwxhji.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gmivzbgka.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gttqhszgw.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjjskregq.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gtqnfpyou.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gxboxdbre.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gybtodwhs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwmecrmlw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/genchvvnm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/ghgmgomkp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ghkungbcv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gqlvxxguk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gevqxralr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsclmfiyw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/grvnthxfe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcmzrkbar.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gqkbooueg.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gywqcgyej.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvyuefkku.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmzgtxzxh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gefzyrxke.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gbaqjtobp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/ghcqbjqty.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghvwfpblf.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmkjkesiq.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gqggmcxmd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grseqtfop.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gztyhxits.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gkqyqjayh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/glxtaghnd.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gcsxsoahg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gnzzknyka.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/goeiiauxz.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdlqldldl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gaigrjckp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ggjrcsgxk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gltwvgqzp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gkwsbpnmg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/guyzoklnw.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gwuvxebch.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/ggwgnewth.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gjikoiziu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gjwlgnzwl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gxufgqidn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gyusvjcbd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gbajkcjyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/geifeheen.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ghluwxdlo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/geawebxst.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gjqkveyrj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gxjtaclcb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gutywnjwt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gyzzewsaw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gjyxxgrrd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/glriunknt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/grqcyfqru.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/guicmsxhu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gewgugzie.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdaqmel.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/geidcjlxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gmejytyby.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gqnwmeqhy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gzkqwpzuz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gkobqdsyr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gcsairpho.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gerijpknz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gkrnihaip.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gqhtmgnzf.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gtfltimvd.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gpbuixywt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gnerxmglg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gkdhlwyna.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gsrxdtfnm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gpzloclra.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gjggtjvms.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gndasvtaj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gbibhjcqe.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gsmjvmqjp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gnrmpszwb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/giogvcbvq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gvowysgly.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/grqzittat.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/ggquefstb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gyzokgfef.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gqhjxxsaw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/ghikenxek.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbqestafw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gxwacsckj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gvqqlwjas.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcmrdzwle.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsyrgjefr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmadaitwi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ganmgkras.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gjzzpjgjn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gywyqiahp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/ggfrrniep.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gstaxyobx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwjdfgbzg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gvpzeoycd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ggnmedvfd.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gdxmurxdt.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gizmdkctf.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gfuykiqjp.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gjlmfvewr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gjpwfaxfa.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gxhrybbor.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gwyxwnvpg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gkqewtuxv.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gqzmjmcdl.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gctquidzf.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gnpnyyepv.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gvoutgxvh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gbcygufba.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gkkdgnrrr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gjkzovpll.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghqsmiufa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpfejfv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gblyzryhx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdmnnnp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gdntmztnn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gaxekwliz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjckngkkd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gmalvwiwe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gkwjuwjev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghfclyicf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gscyjftrz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gtntfobht.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gqsurvyxc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gkzbrsxlf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gaogdhxzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/grxyvmite.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grvzgoozp.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gmfccqman.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyrofopqp.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/grqbanbmy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gkhemypdz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gttwdcrbb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gxukenkra.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gpkfscuvo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwoorrcxn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/grisqrqie.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsswpfuqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/glklgsmef.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/giinfdpqm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gnprvobup.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxahhyjpc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gssxkrkad.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gvfoqwycj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gplqhaysz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gywkraayr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gbvnogqpw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gfbkxgakm.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gvaouepop.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghkmsuexb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gcctgjozx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvogztyab.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/guwdzxhtf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/grhchzkzg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/glzsbsrkg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gpzcsifxj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnsniebkv.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gcwtfcupk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gipejbclv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gtuesrvpb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ggjnskxzx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpabyqvda.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gwbbbmpgc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gbzpkvdbl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gsuxmwlmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/glutouyyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gjavwngsv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gfrnqckii.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gubduvrpy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfhknexxm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gswdlygqc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ggadqzbzk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gvupjfjak.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/glbtjasvc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjsrlobmi.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gkagwgbpf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkcltppea.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkefmbtwg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giywfldrs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzsxhkarx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvwxangwe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxknhtqxv.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqpcckolm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjlenvnhh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gjogfbffz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gysgrwrqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gpkoxaexh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjjcgnwqb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gbavsvcrx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gzbjjkmen.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gqhbbhkvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/grppbvgwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gajvfpwyn.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/ghojrxrwa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/grpyrrldc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfptevybf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxgwetfdb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gomnyjnsu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gktsfxkch.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gdlumchbp.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gvcgdsmhh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/guxmjtpzp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gialpmtos.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdohuwfsn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/glwwtdugy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gqwxmsaoc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gomomvhwb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gqqbfmjkl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gilvijpyw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqxqctvgc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gjdmikmiu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gylrzdrrn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxnwoeron.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/grydekqqk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmlpjdvdk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvknupbjj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gjzumjnfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyabzwujn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/glajbplbk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtvityavd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gcivsaizd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmsxngktj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghwickdkg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcwdqploc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gcjbmghrx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grsbhhfmb.sHtML


<!-- 参考信息 -->