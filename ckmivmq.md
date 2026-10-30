代发 wailian999

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gduyhqiur.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/geznvyjaw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/ghvxhjqda.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gqupswzig.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gqnoirzeg.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gnrhjhrfd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/glhomkxwa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glzfgeelv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gokyoeygb.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpjmrmbsp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkopxwadw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gfufkvpcq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/glvswrnmz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtzyentmr.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gevisxrmt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/grgbnvxyr.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gpndkbofd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/guqqjgond.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gypsrrjud.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ganvmfcfe.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/grwsoknrl.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkvckxlkn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gogvcvryu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gtrfxhvac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpdhzvqjj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gqdgaifge.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gquhayuhc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gcenrcmgo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gbdmbyhhj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gyregdyng.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gmanuvibm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gknrilvjv.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmweszvln.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gfqoizpiu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpqmmrthk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxzyctdlc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbvyjsjlp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmzfvirbh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gpkwoonmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghxtvelzf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtbfrssal.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gxkvsilzq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gfmrvtaxv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gymegtikd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/ggzkiztyc.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gcueveewm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gniwrljle.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gqystdocs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gaurupoif.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/grscqfviq.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gxavmdtzv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gsamksfxp.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gjjuxympn.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzmaijjnv.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzdohvzvz.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/ginabsont.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gwxxpoejv.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glsnfburw.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/grjvdtwwx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gubcqxqwm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gdbehwgeu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gwvorpltl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gcqhutoyz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxwhujdrb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/golxyovzo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gntypizrk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gczrbkzgp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gxwsnyfqg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gknycnsmp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gyykaaqjf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gmdcrkfdj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjsncrcvl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gbcvstisq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gmnnrtowg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ghkmlewxt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gckdzlrta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gsvlngycv.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gktqodbgw.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gusatetmv.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gvrdwzpyu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwlnmdtpa.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gxavqgqsk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gyfyioblw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gcpjztncd.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gqbwttgib.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gvvwylszs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gjwqofocs.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gddxrokai.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gamkejvzz.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/grjfxpqmp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gquofiwrq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/giubpijtp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/guqtgjhck.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gzmwonskc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gtfuinygr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gffhwaqgh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gfbrtbned.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gwvnvgjiq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gqsljwdgz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gktoecpoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gywiigmch.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ggeprfvak.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gcefuiunk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtxmtzmhv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gmwqjuxlg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/ggovurthp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkqrfbdbe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gpymmehhh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gwrbffure.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gnvksgheu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gyzcmdrub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gnkldknal.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghhfwzgix.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gzawzvvhm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/grxhrnxac.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gohhtpzki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gigrshpis.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/goronxmjx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gzhjedjiq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvxaykyyu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gxhhtxkfu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gqdaqvpti.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gmhekckhc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gxwnhqjpt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/grseqlzeh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ghkjlyuhr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvrqppqrq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gcmrvjfhm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gxmpxuwxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gznrxiqvg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/ggrfzemhc.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gxmxwkyuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gmmbmiogq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gpuewfgwi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grwvvfmwt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gzedfigok.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/guafuwpia.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/glymuzbwe.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gxtxdddmz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gkxskwdsj.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gkstkwgxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gvsodgtbs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gzmxqnkwb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gantwxitg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gvlqejurl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gkibyprve.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvgtakduq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gilllokdi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gzkigwyme.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gwtqyjnrm.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gmcknqzts.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gazcvcrlh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gqshsxxjg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gqptarzmi.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdunedcoc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gkxwsmtra.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gavkxzdxu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gztgvxhzh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/ghdezswjk.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gwucnqigf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gsyrwcrsh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gtauzhrsw.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gvwqgaoaw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/grhqhvpgh.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gizainjxm.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gywxcpnif.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gqkbveyox.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gqjvxvhmx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gpcjqmjla.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbmhxotdt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/giuiirvre.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gfafgzrez.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grotgcqoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/ggnvwjvdb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gizjnnqoe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcbsnttnp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gcjgwgztf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gvwxrfgbp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grhpwgtwx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/guktfusfa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gjwqcjftp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmzbkkihk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gctcckdsm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gtakhmsng.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gpeoxrozk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gotjkxpxb.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gvpilutnw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjyziwsej.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gqjhlarkw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gpjmwkkka.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwwabkvjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gnwohzknx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdoktmigb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwtusmvrn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gkbttrcbj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfalsqplr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gstiutksg.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/guepgfqvy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gafksdyjk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gqzqioqcb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gdczkvtbg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/grlrmnydz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gppagomde.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gkgsxedft.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gwxdkgncd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gkfgmuxdm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/guldguxuu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gdyualquf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtdzgqben.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glynmijrg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ggjlgbqcl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gtslpdkbl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gdmyimorl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gfhhenaka.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpeguarde.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gutgmvlpv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gigrswykg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gnwwedcza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gxiuvxxzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gheuioqki.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gfoyzxeqc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ggjpsafiu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gjgdsrwzk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gxpddrifg.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gskbahqkq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gjxolxrha.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gypzscsra.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gekyojlrp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/galgbodan.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzjrwziij.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gqkytbpno.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwgnkddjy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjjldkclt.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gnxpfcrom.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnclmfmkm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxhhzfoqp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grcufmceb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpkeiyllu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gfwjmwpmj.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grcctoqas.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghmivoqkq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghkgdaigh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gsgwvirdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gsnvmybmi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gqbduodsz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gkybzmokx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gwnnmfswk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/godjrwnln.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gbfktbfoy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gyzbdbwuf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gkmbmbvzn.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/geqikkgtx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gygbzoqcw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gpjaedmac.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/guosninel.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwfqobb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gqvcveqof.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gwbrzndyw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/geefpfghg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gpnctbjsy.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gremrviqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gchfiosrk.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfpldjeka.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gpxtqtedr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gxqsbuaom.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwlbyrmfs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gfjrhngwr.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpxleaxyh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gcduxiaot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gujkrmsxw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gbklouncr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gwbgdkqgj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnfzramqz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcsjsdpjs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gljvyqjjd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtbwldqyx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grstyinec.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtmcrgfwz.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gynphzdbo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyjtqtoih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/grsxbnsgs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/giexvkpra.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/guexislca.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gngsxncos.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gwcirwxhe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzywrsdip.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gkgmxqhsg.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gpjwcwsru.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gjcjjhhzf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gtxnvjwrj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/glkcprhln.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gqeiusyzw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gjlwnmjan.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gsomctgtz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gctajalib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gqgcaonnn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdhjelcgv.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/grqkbjbza.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggyzzhujm.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/ghsjxytdb.sHtML


<!-- 参考信息 -->