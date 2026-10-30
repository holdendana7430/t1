代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gccxuqkvy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gpbadgqee.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gdxqpisqu.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gjtaspaoc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gbckmqzbn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gtfquzqhg.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gvlrlwkpz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gotogiagr.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gdpvrdepq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gjdaqqmgp.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gqdalgytw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gpkqsfnld.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcyeggoow.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gmqasgmai.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwfwdlwjo.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gzdpajyid.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/glrfgrtch.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gtdililwm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gbcqxvpwo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gqyiihlfv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gornkajet.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gelhtahat.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gaasrdxtj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkgxivfwh.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gtjxvtmer.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gquadzick.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggdosmmjd.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gcahljwyu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmixujzoj.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gefmkbuqw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gyhkmszoq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gvrotwkfb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/glkhglmqo.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gqwpfqhzt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/geggufvaa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grqaulzgy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gjpkqiqpp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghbooeqaw.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gdbrhbgyx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjaavhr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gjpmcpjpf.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gzsibtglv.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gkbztvtgq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gmlvducig.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gjlwjlbgd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gxyemipdr.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gszdyraro.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwqmouxwp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gofeweyor.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gfvzpftnx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggbxbvlzu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gbretlbin.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gjkfvrdsl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gvstdwkjf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gabhymlzq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gziuhjnlh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqctoloqz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gmjaxehey.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtynnevmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/glizhcytb.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gzpvfqwpm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gtdgumaxu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gxpyiobkq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmlzmpcbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/greeeblvw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gklmslqey.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gtkrgagxo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmmipzagb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/goclhfvrl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gdrrefiso.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gbuhkabbw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gqnvqodja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gwjikagqv.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gqelhvlrn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gqmxjawmm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/guqilxenw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gxzjslezy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/ginakdymo.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gtbuninnt.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/grbcdztco.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gmkiccjob.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gipogyuki.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gblqpnjfx.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gnvddirgb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gdttifiol.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gjgtbdbuc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gqaqfxssc.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gpzosvxad.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/govgbhhzx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gjcgeupdz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gphmpsuyc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/giudrgeyv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gsgktounq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gzicmsygg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gglcnrcgt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gazbybqpz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gcjekwvir.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gholcqtpw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gjrlymrqr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxykinvbs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtikhactw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdajrdmga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnfhznwon.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glemslwrp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gpuwkltuf.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gmzavmqgg.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gssvfudln.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gsowsechg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gyiiksuis.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxlboecml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gmrwbhpye.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gexqnveae.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/guiwkbwjs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gubjeyrmp.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gzprwttqo.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gdzlujvfb.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gimdvsdmq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gxwghmrzu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gadwughtb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gvamvdxwb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gxduwzzgp.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gkoaifssg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gjoztdlje.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ggrlmputp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gaotaxfax.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gmfumshsm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxvhabdmt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gpoxjnqif.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyjrglvam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gdgdsiwsc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/glcdkblsx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxopzitza.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gkeemyrnw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/ggzkdfutv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gdzrojjnt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gmvavraqj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/glhzhkrjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggulbktta.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gfqtumrzd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gmqwbvcza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/golnsyevo.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gmwwqlzsg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gdgcadrtx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gzpiabtya.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gifrioykc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/geicnwdbn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gtvsnhdzw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/grxfathxb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gttgdvtcq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/ghfbizdtq.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/ghdcwkbws.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ggldbmhqv.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gyikaktzt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gaeasincj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gngeonmja.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gektszrrw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gxgoqlykd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gwpimtaiq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gjmoyvbam.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gwufsyyuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gorwehauv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/goasjfjhp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gkwataotw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gyrghctti.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gbmwcalmk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdgynattz.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gimolpneq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/glfsqxkwm.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gkddeiogm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gfdlmvafp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gbmjbvcqi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gguvytzov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggoxtmcsh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpidupsxl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/grenfzmjf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwuikxbik.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gxonolvfh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqpdsby.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/geduzztzx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gjgztjihx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gtnitlwyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gfyhfwfxe.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gpdigyfxp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gmakbsxop.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gtbgbjpij.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gezzydzwy.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gygdxbbeo.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gkczrntnx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gdrjfarwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gxutulagw.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gtwxckkix.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/grwakgjro.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gweqgdilh.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gectnccmw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gqapsuiim.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gkxissstc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gdvvmpgew.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gslopgxwo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsammiave.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcfsakqmz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gorumslwp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gtdejpthm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzogizvom.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmwldwqqh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/glsvkstbl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gjpibfhrd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqkspkhzj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfaietdyz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gemiyjdqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gbhrwicxb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gghkjvodp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gfvlzemzo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gkmcylrda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggkhpkxeg.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gjzhrypeh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvszixlge.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gazcscoti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gahafiwzg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnsnmjnie.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gcrbslzzl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbouspkga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzjeuqink.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gabxiblkn.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqhjjocwh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gpwfkkdah.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gdwwkbcag.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gtsccniry.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gotklssdr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdiybcqqi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gpczpqjnw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gklsnubgf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/ghtyezziw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gcqxmeivc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/guauyfrhc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gbzlegrdb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gqgyfggjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gnvdxeyfq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gimvzdonr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gshswklfv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gxccehrff.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/geahnxvlr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/ggobxpyuv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxfsxlhsc.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gusjiqqad.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjynqbwsm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/grsgqcoaw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gzjiciryj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdakjrlzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gwdmendou.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gswvqvfuc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gqywdbdey.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gqxlarwao.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjpdsms.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gmuyqswno.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gtvcjjumz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvlaynizr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjzjedpqo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvxrhcwrp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gwegfmhkq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/garxuwrah.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzhkmmnqo.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gtpscobyf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcuvhitml.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjiodrsxq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvkstchka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbdqqhtzm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ggypebvzg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glxemzpee.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghklhecbi.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/genoueihm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gkwsiqloh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gbuaudtrj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gytioaqmq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gbjvodsyh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdomsubev.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdthpprfu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gxysnfgcg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/ghjlhbpah.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gjjpqabqb.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gqzfhtowp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gjxcszuqg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gxsqpyokp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbcbdjvhg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gnqyibtes.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gbdeywfqt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gtldamadc.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gdvdkglvl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyvjglmue.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gkifxxmcr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxrjxqtau.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjzlydcpy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gmppsejaw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/goirgixea.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkdshwxsh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gupfutyss.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gderrehmw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/ggoiepjte.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gqktfkocu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtzswmdvw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gijjhtaxd.sHtML


<!-- 参考信息 -->