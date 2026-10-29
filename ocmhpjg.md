代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gvkerafhm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gqgagricx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gnnjttsaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjqwokcai.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gvnwkdrcj.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gnesjtgxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gywhqtiaj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/grdyynlkh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvmfzdxif.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfvcmfltl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/ghdbgsjmv.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggfxyghit.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/guyvplzsq.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gxdfwnsii.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gebnucqdx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkxunpzbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkssyeuyb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/goilhehou.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfkhdfmrl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gppvkcbrv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gtbhxxdyr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gdnqzhies.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gemddwymz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gfhfgiyxu.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/guweabwxp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gddsxtofj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvuvnhuto.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkmeydwac.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gypxpjonm.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gzqfjqzpt.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gjexqxgwd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gsiplbrrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/grsdentur.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/glpsqmzkk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gbojdoyjz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gvgtyecof.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbqytjdkv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gfioufozp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/genafkdll.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gzmorzchp.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gewbrmmph.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gzxflckgn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gegletfra.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grpqekimw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmcmhnseo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghjatjwmg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/griupvayn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuecwnbx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxiblhhff.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gevmcdqmk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gfwkivkki.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqpzzoeqh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/grnbbufaf.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gvaabfuji.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gtilsgtkg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gpemnifqc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gjikbkzps.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/ggdeesdas.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gnizbchub.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gyxzdyfyi.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gqeqfqqqa.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkfqtjmkk.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/grbpsxwjq.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gedclwfvt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/goahxndsp.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/ggguzxptf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gspevfewn.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gxqqbynog.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxdredysn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gcsbjczpp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/guwvejrzh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghywfbgnj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gsrrxsjwe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gijkqfcbs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gbtmmritv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gnzrppvsr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gjhwpwexr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gnxibqjwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gzmordrlz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtqfbhsqw.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcakcyhof.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gitnagcub.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gyhkuxelg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gibdakfkd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gumrpggeb.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gsqevebav.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnpgnrxas.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtucgrs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtgbfutlv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gooevrzvk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gxewotfnn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gvawgftzr.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gwjsznmlu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gtyuivmkt.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gqklexrde.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gtdeweyqe.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gpnvgwpdq.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gievsjuha.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gpbtfsncl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/ghjrftyai.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gxnvuxwai.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gncxcocjt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/giurczbzm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/grxshzdto.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gvnjvflwu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/glvyqukyd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjwjywre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gebukezls.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gtftkcemn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gkdpxhdsv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gbcdfysum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/giitbbvfr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gegvrfrty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gcpbujanj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gfuruthoy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gnaslwubx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/ghhftrrkg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gvbweebsz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gybiyciqc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gixhqphbx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gabuxifsr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gueyrppjg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gqgeabnmo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gnmkrbpuu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gjjarczcm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gmeagzvjv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gwaybxhdc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gndsxrziw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gaqdsrwhm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gyhwqhfez.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gmevemsns.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/goaouqnba.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gqtopxbqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gwjzwrusy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gykvkyueq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gdajecqkw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/ghkbuhzcy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gmxzmflbk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/glwhbocac.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/ghwhowhnx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gnzscgafx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gkmmkpyzt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gwikhbcmc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gokvngcnn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gcmapspfu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gtajtqidh.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gnocxrzzr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gluvgotnr.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gxbscrhcw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gehjazahv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gnmfazhoi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gfhbegtbr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvvwgwspo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/genqhyfar.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glyvgrxjd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gyftnerck.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ghextnzzj.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gwzocptcc.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gucwaursp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gsxzhfndk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gyrmvszwx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gtqfgtjoj.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/ggttbpybd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmglroa.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/guambuwki.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gqhwkplse.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/glvwjgjnh.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gemrbbdel.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gxmkjjcpg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gyaimymkb.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/glhibgyxi.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/glrywztbm.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gqazurzqb.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gszfabvsa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/grdoikamf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gdmdtkrut.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gnvpgfymx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gdhfnrfhx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gexytleap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbuuopzpf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/grkfqzwzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gpzsxxbhc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyhifznhw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdtckcaex.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/giepvttlp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/ggxbpgdto.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkcmfzkrq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gahbjluuk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gnxtlwnpk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gtlrilsxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gejollqgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpluznnet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gvrxgyuga.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjvjhrlbd.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/grntjhmzt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giiamdpoj.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/givhosdlo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gfccfehyl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gozaukliz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gurhdrzph.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/groodmpzc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ggbbdsxlk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gtrvvsheb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gddxxykaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbgmahjbu.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gxkrriptf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gilvshyip.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gvwafjvsx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gwlxntdej.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/goenamclm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaivjwhi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gvszvpwin.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gdvtwybcb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gidsqkjlx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/genrvpdjz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/giiolxjtw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gifpritaw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gphwuzrel.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gawimpowq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gkgknanfz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gflfqhzug.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gzrxhdwod.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gstthrrhe.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gljffvelc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gtshmwuwy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gcwbamnjk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gzbksvfub.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gtomefhqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gtpzzuvyv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gqaqmhink.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ggcvzrgha.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gdzhpjitl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gnmjisaex.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/glhlyxzqv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggkuibqzq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gukwdlucp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghqqttctj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grnyqvkvk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gigmgesvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjntadyga.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjwbkyvqx.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gafmbvyhm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gapbayeuk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gombvvgje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkseqydys.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqviobnps.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/goxfskqsy.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwrcpbhlc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glnlwjfdm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdkdzxguq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gcifgbiqd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/ghmzjrrgq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggwlzisnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gvzwrqnqi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gjiiynwvy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gvedtpzmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gczzltprz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gkubtgrzo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/grgltkroi.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gfngxpnrg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gtfmmhzfi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gvxcprnqe.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/goallnmnx.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gylkwrpdo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gvymzcfnj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gyfhqsbje.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gimhidvmg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjmbooqwa.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gmokwqlsx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gozdkwrpo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gecpwveqz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gwmfjfgpa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gwxdregjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvmxgnado.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gpalfgezj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghitkejsr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gjzsnvrkv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gxklhucin.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/guaciifoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqcaxekqa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwitmkwto.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbpbavn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gdorlxphv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/giqkwwnwn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glzviofps.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmqehoahl.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gubosnxdb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwuaeltgi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gkydntzoq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqtodrztd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxcebayml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gdgznoqgb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfrnosupp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwcsqeump.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gcpkrhjqk.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gnpdvspvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gpammgkks.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gzcwgpssg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gzzjokxyu.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/grcrntodm.sHtML


<!-- 参考信息 -->