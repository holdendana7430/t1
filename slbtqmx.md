代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gcrikxjke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gtxrskrsn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gtfqaykgd.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/grhycsweo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gokfwkzhk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gkitnmxny.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/guwvnqhqd.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gavactmgn.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gcazmhcwb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/guukezckh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcbjfugww.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gjigdxili.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gawvexzbd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ghnrmxlyj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gntkfxygc.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gsmotlmty.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gnztvslya.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gqlkvoopa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gpjyyqdgd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrziulcw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/ggwdalzkq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/garurpdgn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gkbcuupev.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkunuysl.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gpmquwcmh.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/grybxhxbp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gukmlvzxn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gcdjimlda.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gzshivemm.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfyrivoxo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjonubrkd.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gfduemqrb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gvdwyvgug.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gisqmxhak.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gvmwzkpin.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbkkqavff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnjzdkxec.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gsnyezfjp.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gjvsysujm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gurhktldj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gtcujbsld.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/ggzekispk.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gdjxwkwzg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gywplcefv.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gcfczeuii.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gmjyglrfl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gulzszegy.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gnkgvxvkv.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/glzdcpnmg.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/guwipomkn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grntcmxbm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gnrrnqvzm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxxkymvdt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gokuxylzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ggmedroug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gneorrsth.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtaogjc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gyboloxjt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtarabosv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gdwsidsrn.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gladzraxp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gvpwshkdz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/guywltdiw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glotzziee.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvjensvts.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmykbcmmc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmbmpxmx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzkwcqpiq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvohrxlmf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gaxxgxpbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/ggqopvsei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/guvsrlgvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gxrqlsmih.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gtagfdjlr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gewsdjmed.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/galqdcsqx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gejzspuuy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gtgowpouc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/guzokrqlg.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gbxudggzk.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gxinexavo.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvvmpdyar.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwdcmrllp.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gokrtuazx.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gbsddvycu.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjqijanxu.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gukacloal.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gvdndkogk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gjpykyqqq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gkyaxenpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gwpctgcnk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gddltbsen.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gmykdwius.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwivjczts.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gxjwywfln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gbjtbsxvo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gdiwknvje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gldunoszc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gcdvezkwb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gjplobgqy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gntcwthua.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gpbseschv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gvymnctxm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gfgvcjwlf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gebqnsfjo.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzgpgnmse.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gdjvkcsxa.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gnwnwuqik.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkxszpmyo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfjvmufxf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gxqrhjhml.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gkwloctvf.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gfguhcino.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gnakmjnkd.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/grudmuazv.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gekpfaxbi.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gdwrcpeuz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gyszexbrv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/geqrmmgwr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ggieqivgm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/ggpfljqmg.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/givglnkdo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gbqxxrvel.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gdrjonscl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gxvqicaeq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gwghunlhr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkqmwtkpa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfszwdih.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghkylajqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gkhqnzltn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gqmdalnor.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcfybbjyz.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gurrdhreh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gnymisclq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gwwswdaox.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gctaujyka.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/ggjjzduhr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/garvckeoo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/ghubrvjxx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/ghwvszjbw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwjmuazzv.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gutwvhqle.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gnkxglabn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/grsxqxyhs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gyzbppuri.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwkzykxen.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/glhtaauhl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/grzjziuar.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gadoiwxje.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/ggrqjfxxp.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/ggpcyxmcr.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gpjrwsuhs.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gjidsjogv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/glksepfly.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gikcwwcwd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gdgnkupcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gtarsimfa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzpittehh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gkvpgisre.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gywtkwkrn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gpxhuqamr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcweibjku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gnjbwekux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goseiwzon.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/glnwltnjc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gflgilnap.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gswmmjpfr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gpnzkwxbd.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gaaussyje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/ggneazrib.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gukdtwhjo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzqqewwkq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbpvkciia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtbqcrehw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gxivbhlzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gdnhpgeol.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gdhbqrlkf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gyvwqqagv.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gnbaionuu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gqxgbkvon.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gpnovujzt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gbaaaozml.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gkoizwtqp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gljlyvjxj.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gaktlojop.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gdyvypdix.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gapwjiomk.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gbuairrzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gjvhwqnxz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gqlawulag.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gxodfmfcx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gwotdzfwr.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gvmlnxtme.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gegxijeko.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gnlwmnwjh.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gdztlbnch.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gnantzbnv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gumelbzvf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghncwvecv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxmbnglra.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqxweyzua.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/grlxputxo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gbnnluijg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/giunqtult.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gcxwpbxct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gvveyzsvj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqfczbnmo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gdvskzwng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtvzmegvm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gfgsparqo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gpinbbgbd.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gctdnvehv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gzrhjujga.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gebsprgco.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/guvnjvxuu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gffvbctzp.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gvmhievnm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gdduoqomn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gthttrlfe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gkrbuwdqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gxctcvpkv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gnramrqgp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gjtxetdgf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzuemfxnr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzzeknncg.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gdfuatgaq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gepbyvckn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gewzljffy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghmbemjuq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gptfksrhe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gwqawpcul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gkydfppvu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gmptltzwf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/ghcyvhkkw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gjgazjfet.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqjnabndo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gnimxvuoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gdyncdnwu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtsbcera.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gtnrgcmqd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gqbzimfvl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/glbilarct.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghciuoerz.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gbpsawrjv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gobvskdpa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gmcyfljra.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbknjaw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqsezmdun.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gndsupgrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gddiefaip.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/ghhdkwpru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gvssawmxv.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gxrzplrao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gzrmjuhql.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gphxawlgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwxopslte.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwnbwgspq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gadeurhlm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gagmiandj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gthtsbois.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbtepoflm.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gjrxomypf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkdnknnlg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwqoqajth.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqsrnplll.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdvadperm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gyorfnzdm.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbtahmzlk.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gidgnlfjm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwhdkulut.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/genicgfku.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/goacgkzpv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gwezcrqtv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gtkxecxsi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gxzjfkhgv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/glssjpexo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gxbefsung.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/geqvwpjtp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gkyciyfvk.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/guitlpebg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gtsenfxlu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gcakcyjgi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjlmjppmy.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gmmkugrhf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdjekdids.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gsakikthn.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gurfrrxne.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gshgqmkmp.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gwevrumfc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gamlxxjsx.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghaozoanu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gdlrvruan.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gyvaxlodx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gegufzkhx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gwrkdnkob.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvwdcfnyz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gerpqhbcq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gguhdtuej.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/guczwafon.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcddfzmfr.sHtML


<!-- 参考信息 -->