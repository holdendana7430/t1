代发 wailian999

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/giyuuvymo.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gajfagain.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gzcsmthar.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gnbabayqt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gsyepwdwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gxehokfuj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gobqsxghl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkudouzkh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gcjxoinyo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gpsyxuwsb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gsikmlcux.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvqexxzux.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/grprqmsty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gjpcxmtzg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gpoalhdze.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gzpkonwzn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwsegwrew.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gosdgqfei.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gtmiibwhw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxatzyrls.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gyhmqjbjt.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gxvharanq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/ghgbfropo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gkbyqlfbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqlmrzepp.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gpvoeocdk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gdxkaiaau.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gzukarign.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/ghbybytxi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gcxedcgco.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gpbyjgzxu.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gwvvbnaoi.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gcibumisp.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gbvvggatl.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/guexlbsnb.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/grmdrcikr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gxczanumc.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzxtbylmv.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gtaisjwfp.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gkdsvdxba.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gxkamhasn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gryucgmzl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwrxmmyjk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gnrxorlje.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gnrhfoajt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gaqscjvel.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gnwdykkmo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gfqgesfcw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/geksspjnl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gartfiveo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gughklslm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjgaiinvk.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdmjjxsvr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpszoxdij.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gfbndaxos.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grrrslxgn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gpasohiuo.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gugwhdocc.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ghydzbasr.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/guzymfkqp.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjrxdhylo.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gxsfeklpl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gtdcumvmd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/grxqmgrvc.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gaaloghvc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/glqsburqw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gshebvibo.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtyyzvhwt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gshijlzzq.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gvkfyduwu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gjiwklipm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtpacoyzz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gzopvlpxh.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gyjfpflsz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gjwkerobh.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gumljgxea.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gfkouyfpp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gslvwhgls.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzjoyxxlx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gjjhiviyc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gvcpwkyxo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gejabfshb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gklmhdzfs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gajpshzye.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/geygigscy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/geraznujv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gpnubvgif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmlamls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gztlgybwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gahfdwkhi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gtbnruwbj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gwogfervg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gmbxdqsfu.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gqzeegmqx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjhtwkxqc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gofmsxdqp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwyfhnwx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gshsczjtf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gpmodlsde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gusvagayh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gseiarxfh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gtcchgibk.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gmgezvmqe.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gwrmmjjiv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gzzsuglqw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gaunultmr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gqhriybfr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/geojpzfvh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/godrcreik.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gcbtvrgfs.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/grgfcrmym.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gfwwdiqje.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/grkfuturu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/ggapixxcs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/goohyyrhg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkqofkgdl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gowdvpthq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqdizzafy.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gxcbpouiz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/ghhxowiwn.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gruxavpho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gipddgvzl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gsrsysudg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggwkaoutb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/geyvcnfel.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtcepaxxl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gabtyizjg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gtncasnws.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gclmbqkmr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/guifplyji.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gxfkffnfi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvsgqirtq.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/grrdanpsw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ggofizyae.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gfyzkchwo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/grobmtrjn.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ghuktdlko.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/ghnbyrdtr.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gjbilkmng.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/ghztqtnim.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gjudljerp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gfvjfrspp.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gkdzbonug.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gtprelwpk.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/glffodxbj.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gchnrzgtv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gzixfzadz.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gklezfuso.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gzxsbrevo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gskfkeeml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwprndgfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpnqrxkzk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gxjdeccbe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gtluaosyp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzqnyngdn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghlfvbebj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/ggghdvbek.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ghmakpbkt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gckmcymir.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gwkuqhclf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gtejqluky.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gbaqsnxtx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gmuynwxwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gkwjtfiow.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gofbwxroo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gffbharzl.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gtjevoxwp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxadsxgpr.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gjpdpsxzd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gsukjfknk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/giqlkpiru.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gwkrqdqpb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gkuzrrykw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjwowwebg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gcbmvwenz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gebrqxsch.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwubgsndo.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/ghexndxtr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gnpgjqeif.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gybljmfjj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gktcvzxhz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gbvdzhahf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghyroziwl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gjkyvvlda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gupyngvcj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gvzcutyso.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gvfkrqlfo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gmyrejhps.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfewdacvp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjsltjaxq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gqwdhtzgo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gvwkjrwbh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/guuaplfah.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gzohnmucn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gwonykxwv.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gcmbqebkx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gsumdeaue.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gmdqifsrr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/glepllbne.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gbtmybece.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gmmskscym.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gksosfsnb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gwhxnwjff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gcahwrwlm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gsjrqxacm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gvxmfpqnn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/giryzmzio.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkbqwweyv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gozwtqazx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghqpnzziw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gibuqtejv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmodzqfgr.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtuswwxmg.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gohtnxayk.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gebtedkhd.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyvuungin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmbzmnddh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdtdlqhhj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtgiyxrny.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gruazcacy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkarkljru.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyhxmltxs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gprgbgboy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gcihpuoab.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gltdudgir.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwrncmhys.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/goedpwnpj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/geabjbhgn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gbpjgvhlg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gpmbggwns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gbpelskah.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxspdtdmg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gitsrtofw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gsnkacpao.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gjicyfovg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gabmfjmzs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/grkotjnmi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjxytofmj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gykkrxcmr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gybdwqypb.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gzigdglrx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gehuulcwy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gubfswcww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/ghpetsbym.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gpnluhpbm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmhnclhsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gdxblwbss.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbjotqcgb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gyvwyuzst.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gidpyltgw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxfxtlgzf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnojyeohn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gocwudlvr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvwnwqrmk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gblvrrusp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gnocmpcav.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goykkdbfj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gksyjkghg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gmuylvgxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gymqzsaeh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gutsdsgnu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghzjuvkkm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvtddnorg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpgchwoue.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gfyiorlju.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggpnllgqq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/giymraajv.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ghbzejeak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gmhyijvyr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gpylbwkmt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gxzlnseks.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gtfmiqfnk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gwdgunrcj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gwncfawcs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gigyquynv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gvfdyaghz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gntoshfvq.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/grynzqjrx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdxbkzguj.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gxjbhsyjp.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gejnnebma.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gakprjptb.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjgofyzyq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gxjkbmvxf.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gixsydlex.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gazuzzhxt.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gugvivreo.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzmjlgcxf.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ggsduzlyh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gygqxwjeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnnabyksz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/grshpwljf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gnccivmdv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxvvzgdea.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gruqgkjjk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/ggolmdxti.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvxwbncxj.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gebboflcb.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpijhunbz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxiyhomrp.sHtML


<!-- 参考信息 -->