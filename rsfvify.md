代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gzqonduph.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/ggaqudnak.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gpeobncck.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/godttkcsk.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gruvdsmgv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gsxypakej.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gvkvbdzan.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gadipdyzs.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gsjuptpjx.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gqiwlafou.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghoxcpoai.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gayktfrte.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gpvjwgzfl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gyxbupkrd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/guzfwmfxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gxcvzojlo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gnxhecpam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gifrdymud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gjdakitva.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gedpnlujb.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gfwxrsfuw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/glkywcekg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gnmtnsuua.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmainfehx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwgqgpsjh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdoahlqnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/ggfvitiqi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmjrptddr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/griovezwt.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gqaisuvok.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gvzlwkfxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gguwsphor.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gaynitkfo.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/ggzcwmckt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gqdyolomt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjupjigag.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gawjjuebg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gdziroirh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/ggfjgffac.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gmxkkthve.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gqrchqotk.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gdjgjzkro.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gobtsqpzk.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gvaqswgdl.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gkdnnvcdv.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gltdyimds.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/goeqbized.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/ggnggsmks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gakzzypmh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/grnzvsrqy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gzmxfmhsd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwszmwstq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/ghjwnhadf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gcfdymhmn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gcezftoew.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gmtojpksp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/goqasbihz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbodpyoes.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/guqivwcqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gdmjhliyx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/guhjilitm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfkyxgo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gcaccgqyt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqmjayveh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gjnxsrcou.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmmwvexnv.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/ghrxctvvt.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gwjvajtbw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gywgywdis.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvsoruogq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/glnaoqcvz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gwxomcvca.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxqxnheht.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gygamwuxu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gepdarxbp.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gmmodciyj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gvhejlrfm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gynzqznmk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gczlqqjzm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gekwusned.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gsvqbudfi.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gmtictsfc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gdvcvclso.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gfqnzfmrl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gpjppixpx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gspjzidrf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/giszisrwn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gvdhjpuee.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gtlcwzpps.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gyponrola.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gjlgwsksc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/guqcmjmtd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gnxmsafxy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gzrozizeh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gltppwmoj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gwuipkydk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqpjsrlyo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmghuqgyk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gwyvopkas.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/glosvaqpy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gojaitkvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gomjjxiie.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gynkbftzo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gnxdrcpge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gupxzdoir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/glrbhuswn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/giwwxzhqw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/giufpwydl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gwsmhmksh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqoxkxsar.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gqptblodh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gxrupbroo.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/grkvzitid.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gibdtfgmx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gpezqbjnm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gstaaxioo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gtrompvgd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gsasnlrey.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gfzyapmpy.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gcisquawu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/ghhlnpagk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gezndddbo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gqmzrmthx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxjifjyjp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gtbrfqtxp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gwmarrerj.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gxzbkqwis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gazduwolb.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gfkzqweft.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/goovhiogl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gfpkevofh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gbmtrwvrm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmlwgxhtu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gylqgtqwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gkqbzkccc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gmdpezpyl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gzubcqdgv.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gtqnathoj.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/ggjxenszr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/guryamjfe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gowacpbpx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gjrcwrvol.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ggfcwdtdp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gjpdzlwoo.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gbzofxyge.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gvvpnphbh.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gvibehgia.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gotcjywgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gbinlsuln.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpklyjuyx.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gygmldznq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmukveuzv.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gaciqorif.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gdjngxgaq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gjyuwcbll.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gvxomojah.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gmjjolezd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gugvmhias.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gvlmllukx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqrqkkmfh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkojvueeb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gxfqnbmdp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvovgliwo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gbwyvvihq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gfrdabndx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gcqpgrvcg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghjnbiybq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gdpucuqlj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gemqdbeek.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gefweatsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gwprnsyyd.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gripakotr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gzlkapiak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gugmovawm.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/godeuwotq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gigcososc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gijampyhs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gnwcwmxtd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjbtaymnb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/ggxabdzoq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwgyivcxl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gssxuxipz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gawmyyeql.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjslsrdjp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gehskgdwx.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gnpfrpafo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gycnhrost.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gaxqxwiwl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gsilmoveb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdekyghrq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gcewxxygj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gxzbzlbsr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gxngpzicb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gipcxdduj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gqpgaaaan.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gvjsfaash.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gzhpcdokw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwdmhtfaw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/giauywwwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/geeyvnuoy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gxrtreepp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gyextpzwo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmoebhveg.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gjmvcgjby.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqqzqqgyk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gjpsgobbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxerwowvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gxpwpkcxk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gvbvcanhn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gimvfnrmn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gybnqauuo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/ggoouuuks.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gvnezzbxb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gvwbmppcf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggrkfkaja.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpyuaoosb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gahqhwota.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdfvusvwm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/geroktdgn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gghddgqig.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gekixjhhd.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gxvtqacqw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnvxtomjy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gugtiasvj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvmyqjufd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkfjnykdj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gyfmukbuf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzdignptx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gucnosyfa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtcmiqhbf.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gcukxbila.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gvjbdtyny.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ghftzaagd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gbjxeyjuu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gyjfqwrdc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gbxaalzut.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gkwktsbos.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gjqhmqykj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gtyblrisn.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gywamsmwt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvbpmsq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gyxtgccjo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmpxvvyil.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gdcbicinx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gxzgorgnc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gdrfnklpy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gaqahkgxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gpzgnnoef.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gthpjrdmq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gonkjiscs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgpaitw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/guwcbpclt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghaogbuit.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtxtzgile.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/ggffnspvg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwpsndzyq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/geyhmsvaa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gxgeallpq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnmxotpsb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glnmosnat.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gadddhzrl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbrfeyaeu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gibsjbfxc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grurgwyvg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gbnvvwruf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvfxjsnth.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gwjaqhvmf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzvvuhhvh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gzaezxoex.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnyugculq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkafrdqrw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gzrfytzdc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gbqbftztb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gattuqjfd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/ghxknyhru.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gssodvdvz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gaomryaaq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/guozayjtv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gyjsacujp.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gxppnxjcw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gymwkqvzq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gvwxxnokg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gdbmrvnjz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gvrmklcql.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcarlibyz.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gjueqlycf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbtsvvhvp.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gaseqbrdv.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/grdsqehdg.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gygirlrnn.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gxieshsij.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gsqutjmtw.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gxcaxrocl.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/glaacfyln.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gzybeufjv.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gfodqbads.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gafroajea.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/giksyirfb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/ghiqzpuzw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gcbrxuakq.sHtML


<!-- 参考信息 -->