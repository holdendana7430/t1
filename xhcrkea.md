代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gmasrqegu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gyoqvbmqi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gcygekhkd.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gweoipfig.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gefebckfo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gwsidqjaa.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gdrjbbity.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gukyuouyd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gtypbhehm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gngkziicz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gssefhlxj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gfsjetdww.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghevqrhzq.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/glbxhapss.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gngsxfzdk.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gonnbrmyv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gihvfdfjo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gjplojwso.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/glodmayar.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gsuakrvjx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/geqfnqoet.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gzqvlmwtz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gadcpspjl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdohtmasl.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gypoejrve.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gvmcxtyve.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gsikzbhth.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gurzitfkc.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gogheuxmm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxpvemzmb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gpxnbfcjt.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gkurlavqr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gpurrsahg.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gtcqmjwus.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/grjaxigxm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzejbclzq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gjdajhdxu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gquldubux.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkebtkkpb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghvygytuf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gtycwnxkv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gfxcjvjbj.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gykkgjkcv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gvnketeqn.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gqhajbonw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gofynkfju.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggsuyirut.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/guoywolpx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gelxvikkz.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gtyrnmreu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gcezjjmjt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gumbkmjcy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gbknvpyzt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gwmhchviw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gynubyjyv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/grnjrzrrw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdpvurcsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/grtegqizv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gmhckrpsh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gngwsxcqc.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gywmgmwjm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gpwdoqejd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gljbiohcp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkqkvvonv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzpikumtc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtfksmvnp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gzugzunix.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyjrodjdl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ginmbwlyv.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gzqjlesxc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gwaxtdwtz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcjjkmmge.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/golvxnjgp.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gdgzjwjqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gojgujkhx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gqoheqbpe.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/giyikdciq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gdpwulono.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gxadanriv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gwnagakiv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gmzahctzp.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkgbhvjus.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/glohmyruw.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gctphokzb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gnebjjsfj.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqbgvtpfl.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gmhilpkww.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gehgtbpcf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gobguyemy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/grbaybxyq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gzbikzusn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gkiiecrui.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gidwvwajz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gzigoogjn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gnlrlvnlc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gvxjmmnlt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/goumtrtfz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gdohxjkuk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gonzcpwlr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gukhxxcxv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzwqchvcu.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gfhshkbjn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gczpoouyb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gijaykvwv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/glbxveqzy.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmtboxtyu.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gdzhrfont.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gvlyozkbw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gktmcqonf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfcifsrde.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gnqijvbzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gqauewoie.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gmyzlwvdw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gkfuluqaa.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gfumsgimn.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gapgggowf.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gfwiqguil.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gnietrpbt.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gvvoajkug.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtfvhdwpm.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gmwdkqroj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/girfkhfdw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gkblhrgbe.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/grlvpwemp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/guxzlzptm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gusmhcebi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gyimvkyml.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glgjteflh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gwqbhtcge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/glrjjovki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gtxcjwqjx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxdewnnsm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gcuzaapnf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gzmytmojq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gqdetwcnj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gstrgirvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/geszsxmfv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gssgtloti.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gdhbjkjyv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjhjzdn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggdduhyis.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gyjgiyvvj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ggleoqatc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gymgiwlpc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gzhlzamza.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gftnukrgk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gscicvmnt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gqsxzycfc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gzqfzpgyl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gbexuedmv.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gavcujldi.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gfomeboxb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/glpivsfmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gwgshyyiy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gitwcntow.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gqrpltmwk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkdqscp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/guopcfcht.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gtrooyftl.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gtbzxageg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gcsdxibnp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gbbtrkmce.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gsxudjgfm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gzhdmkupv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gtazxqrkc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gjhomdtqt.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gwcojzycv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gnqzxzgmu.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gwsivdnhi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gkplqrrfq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gjsmcohht.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjgbueonn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkbqfnqrw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjzxqirje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbctkcw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gixbayqfd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/galnsdmxe.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gxiorqwzp.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/grrrbgbgk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/glssxslho.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gzmrbrwkf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpaywbzzf.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxbxkkqwd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gdhhmjyml.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gsgvzhupo.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/glacvgwmb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/giljjqzwq.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjonsfs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gsxddoola.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gmolgbclm.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gfnyipeon.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gvcjelonh.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/grwuqrgpm.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gxnzkwehr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gabyzcxit.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gqxggnouj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/getxuciel.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbhndrpsp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghzqihbba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzvjyzqqa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjtnucvsp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gfuiwupkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gujkhfxaa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpkigqrfn.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gnojkyane.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gdfqhvili.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gyjznqpet.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/ginesesbp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gsokpkgav.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gppsipnko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gybolabse.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gwhzddexs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/glfmvcczl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbojuivym.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gpzgvnawu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gocqeecsu.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gaaxvheuu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gcjfjneeq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrftprp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/geevavfpq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdxkqclot.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gshmgclhd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/ghtxmhxfy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwrmyehsn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtvranove.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gypoxtzrb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gqsfynrmu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gwtozuolt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gkhzkotat.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gsjthqthk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gcgptqurs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gvkhdkhnu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gjgvbsltg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzukugiwl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/ggjmcepiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/guaewluie.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gtfzmfhto.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ghfiwpcvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gilwyebln.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gtstepctt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/ghlktjhou.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtnpeabut.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gmorwpaqc.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gjspuhesv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gqryozlcv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/glafalngr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/guusdqkgy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghepfjcrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gkdknxzws.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gqunwghnq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gytrkvivt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/goitnrlcn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/guguxrotp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gxuwwzpnq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkpdrofpe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwfimal.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvllyjvye.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmvnhgfil.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gdmzqdlnd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxpjakgag.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxskaqqzo.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxfbqfubk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggbietzeb.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggzwzsehm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpxcwywxr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glahywpug.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gutvbrepi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gorgvudmz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggghejzis.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcswdrvcp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/ghsexkxdb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gjjnyyfrt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gizndlzyw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gxzzbdreu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gjrgmlzou.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gzouhpmhz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gfthhktob.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gjyabeiuh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gvfwjnyii.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/genydmvdr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gnlikfqdd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gfudovgwo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gngpqkaaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzrkbxygo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gpzwsmrrg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/ggscjhsvn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gwkbeiizx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgnvkxjh.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gkfxjvxca.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjalkqzll.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnsbhzysw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ggjwdncni.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gxsrzeurz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvmiyiivm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gwtydoqrr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gabiocazc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gjmdiacbj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/graddpotw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfoihemdc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkyybuqvw.sHtML


<!-- 参考信息 -->