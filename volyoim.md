代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gzmlkxnjw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/guwjgnioq.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gnnoqbqyf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gauqwvdjb.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gpgwzdosm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gngsuoiuq.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/goxfhbxzi.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ggvgccwwt.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gelxdilgf.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/goanubafz.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwjdedzlq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/ghkawhzgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gycdoahah.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gzeyaqgvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxisvjuxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gigifxqsz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gaonglriu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/ghtupmmvi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ggjbqbckb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/grfxuzbnb.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gqmasxltg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gojoxxukl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gjsqwupon.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giiasocdl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvxmvjelx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxyxlpacq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gazibmgbr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gecmavswt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggljkpxiq.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gfxjqpijg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gshqwlgmj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gvcsphsxo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/guecevjnd.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gxwfrwmow.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gcyosgzgy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gnjpmhmsa.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gflmwfkkb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/getrouren.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gjqebyeag.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/garyzocwe.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gcpkgdbwd.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghhilzitd.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtddlqfuq.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gfrriersq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gorltaykc.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/godjlpzwv.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gwajlbwkd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gdrycajkq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gyaaulugx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/ggvxplubu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzmbvlf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmtlywlnc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gshenfnij.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gkgtampif.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gubtiewhs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gphtogjfd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ghxidsfiw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gsddzmzex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gtzsydltj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gqjkunpkl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gestiilej.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gisvmklly.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ggzfqgxiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsufycfnj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqtcbspyv.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gfgoperbl.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gzxknvbze.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gstfwthyy.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdunhtgfn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzdiguyvi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ggrhjnwzx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gnbepqwhz.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/ghciuyyni.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gadleorzn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/grhmzjgxn.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gjfmsikrk.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gfjetzalm.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gghvevhzx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gaiknoclp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/geyxmcktf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gixojvahn.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/glexqzfbr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjtrtbrju.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gbskccuco.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gdgnyradx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/ggwjoieqn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gbjubzrwv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/glwbjcjxi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gwbjojbiv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gyljuqnze.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gasyeatnm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghfmfvtun.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gvwpogysi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gbjkryfns.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gkxrxxyuo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/guzdxtmkj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gjnsoxlfh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gtknylqqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gqsjocfhk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gyptwnfvl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpahljxxi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/giosxfdop.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqwmbbgcq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gdzhptrtk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtxmuso.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gekfpbtwd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gybfsyitr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gjcwjqulb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gabltykgm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gvuoekcnf.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gudwjijwr.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gptbuyazo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gsnyfntgf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/grafuvsmd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/geqvboags.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzsyurtzh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/ghqzodqyy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gjeksdoal.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gtclzrrel.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gdfqlrcic.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzipawrsr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gvtnelppc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ggdmelgzy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gebbmvbrw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gyumldtdt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gmokawulx.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gehqnamtn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gltnuwgra.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gytdywffw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gjmqnikmb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gmillhztu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmcovhprx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdtstensc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmreawtms.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gndpajvog.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gfmlmupva.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gbfjcrgnk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gijiflczc.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gcqswadrp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxzasgj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/glecsqmeg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gemtquwsa.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gfniokfbm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/ggbewgior.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gzlmotnpk.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gihibgkvc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gpniilpfl.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvpbghnlk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gvnlnzxsc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gkczlakwy.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gaoyfufbq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gevmayxrm.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gunmfohbp.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/giuebxlkd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gvpqrzthz.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gsqiqrusj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/ghpqgwtet.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gccxhtbev.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gatmjzdap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gxprannaa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggidzlpyt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gtuvkivci.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gfdhhqopx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbsrccdei.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gzjaqqxjw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gbxtaiizo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkwkvvpiy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gylctnzic.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gfrwuxnsl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gegqlgidn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gfdtyowmu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gipetxyef.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gpmwzujzj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goteayeku.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gbusdarvh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggowusaan.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gamngoqtc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gquxqqdqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqcbvdsni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gafjratjo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gscnejfvb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtuyvooql.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gnwcyvuep.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwyzqbats.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggornzohs.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gltfxuoud.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gszxipozj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/goujgzljp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gwokzcbym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gktassnbg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gbdxgjvcz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gunuepehy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/ghsutrbpv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gmditmqgr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gdyjobtep.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gydrybyxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/giotgdscb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gearjrlsr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/guawzfllk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gowiezzel.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gaschoept.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gcxmsvezm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghqvfthjg.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gpngxayea.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/ggxpaazqa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gqizspdls.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gnflywtav.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/grrahazkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gdbrfpscu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gxlfxetyp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gmhohhwqv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gmsarxspp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnsxvhlyw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gcwncwelo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gynqqmgng.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjfcykchn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkrfgykhg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfqdtvhnm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gcfmfeocu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glyxsjdmb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdihvzcik.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/glxviblyx.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gppktwrla.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjfovrcva.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyigrlfly.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpuhufeao.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gymldcvbe.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwurqfszp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gniszqfou.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxpjmoqhl.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/guzpsvhkn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gdyeoyrqk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gvwsejuqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gsysjwhnn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gbfsvvqif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gtokkphil.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gtrkewtku.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gcekcehyu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gciggijky.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gyedcnzpp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqahpird.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gtlcsqcnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/grkmhyjdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gzmaerkmm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gtegbsbdw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/guuguibsn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gdmysrwjo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gtbaxbmtz.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gyoctvwml.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/griljbjwl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gskszfbwm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gsykdgjum.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gzbrvjkll.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmgcwzprw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gnjnciohs.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfibcvttc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/godjfcwdl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gyhtnrbav.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/golnpeavb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghlflweow.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggctawmyk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcwaodkrw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gutxmxpzx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvhnjfjxs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaozlpluu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnmemynsn.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gduzdomqw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grtsninaj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gnxrbbiln.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gseuazfxh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvpocehlu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gpaytpphr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gyldyxzby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gydqkznrr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gnsxanfvv.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/grypwstsb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gyehtoklh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gtwjsfeue.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/geyliaxue.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gprordvri.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/ggippcsgo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gijkxpfjw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbfjbdted.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gxxtmnvxb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvgtpttzf.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gunozkdil.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guclnehma.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gbwuchkou.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gktpvtjbc.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqzkjjaqt.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/ghirlgoif.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gvveydgul.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gkcfanqtl.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gmhwlzhcu.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gzbeocmcp.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gupndmaao.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gwsxmlcut.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbdqzso.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gvjtycjlg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gocbzafot.sHtML


<!-- 参考信息 -->