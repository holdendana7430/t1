代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/geovswgle.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzobsrwiz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gdbzoyvjw.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gffeyecfd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gawwhqjgq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gfdvtmyus.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gfxltnlxp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gezdclnxe.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gyuhiukba.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gnrbxhbnj.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ggxwithrc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gomesugrm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajrajfxg.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gxmounilb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsbwthrls.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gliswqehq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gbdrwckxs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gjhtodvpf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwdsspamh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gsagobqhu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gsqbaxguq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqkgxfkkf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gvselrzhs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpxughcyl.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/ghgwppfzy.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghpicavqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/ggkcdhwvh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gcgwwyiwn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gyijcppsu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkquyxljs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gzmjqmrdl.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/ghnbdxvvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gmiioomzb.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gupdygwvf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gmzbrdkse.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gwdqclnbj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gkgqctaqv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggvbioicw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxcqprifk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gbeoxfjuv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gpgstvvrx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gtoiuxxxg.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gpgjgbcjq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gwjojybae.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/glcqexuoe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/grbcujaof.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gzurtsebb.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gusjicvsv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gnmryturi.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gqzaffgav.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gtqeygrum.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/guwqmcpum.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggdqgnhbi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gvnmwglkv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/golpojfad.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gdovgrdxa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gumkhivdy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/ggcpvswft.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gbanwasnh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gltqohovo.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/grcesuiyh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gonitmahi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gnmtvswrn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnjscieea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzlbwbxmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggtjmdvku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gtrplduvs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjtwwwrah.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gudvwtudb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gvqfckvld.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/ggucsjnpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glcwcpgjt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gpxmdzqxu.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/grkkvqymb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gncbjzaya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gmddigarw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/ghjpvsrqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gmnwnrhlf.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gwjbqfosz.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gqlpmuhsa.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gfqvrwcmv.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gmteeympl.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gphdxqtln.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gtjyvibim.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gkxybdxbd.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gftalzgyu.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gvhsmkkgq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gvsqrhhtj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gmhldcqgt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gkwfmujip.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/guivxaoly.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gfeqamrzi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gouoiacgu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gthdlajxf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gtnetuthe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gppcctsdc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gtnntpvrp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcmphtklp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gdzppsgca.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gdshxepux.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmwkxcuuk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjcmdqguz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ghacfxyzf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gvgtvivji.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gmmfrjpqb.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gzmssjtzp.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gfgpinkbe.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtjzebfxo.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqiiivkjl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/giuplpkuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbqowniic.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkqjnzfwr.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gtwbmsqxl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/goecrubok.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gntaukmlv.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gexyjefcu.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/grblsaecj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gzwgsxqzn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gyoviszgv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gimhbbsvt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/giqgxlgtm.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gqgndappv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gutqeoirb.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gyfzlwweo.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gbwlhxqvx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gyjeqsprb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gambnyjom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdnwabvcd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gnubfcene.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcozfoxkv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gsovqwtbu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gejvbvkdq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gavjmnbdx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gthhvjaky.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gulavegyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gexzjxzzu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ggoatkobn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gswbcggmr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gacdznoqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gnussmgbo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gkafufuod.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/glhyhmnli.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggeehyukx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gaypszjxa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gktslvaoa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gmbtjnmxr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gfrreblia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gzhlelyjg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gjoszyvul.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gcuvdetqf.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gxtqiachm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/grckmehpu.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gdbejdmob.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ggwzkokry.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gkigayoma.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gnuymtksv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gqusqgxyz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gzzbfkeie.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gvogiwbjb.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gfvrsapdv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/giaswvjfd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjifskad.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gyhswsqvm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gbtyrvyhd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gszknbfyy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gicxrerua.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gvsmcwayn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/ghtruomyk.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gxwppkgzt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gezholgso.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gzkvkwytj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtkiwerdv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gusrazwhj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/giymiuoul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gucxmwbtd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gcoiqwdwe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gfaracneo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gumkbvrrk.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gmjgizigp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gezxfbmmc.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjbdxsspn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gqnzgsavs.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/grigotdvh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/goebqxybb.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gyfajixbc.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/ggsigptam.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfhtddbbm.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/golrodniq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gfmyqqukp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqlnsgfcr.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gobabijco.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/ggezyhvcm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gfrdeplej.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gxcgifhub.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gwbjwteav.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/glrkdhoos.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gdhkovwnw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gisqniekf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqlpoaebl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzkxsefpl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggnlhcqms.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gnrkkxeie.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjpfuaqyl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grywhzsqz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gxlryydkl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gzxgvvsde.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdfqpuvzz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gktdnnaai.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/goacaihhj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxklynvmb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gzkcnxsme.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcclfxtcc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gaaamrokv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzluwxujb.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gghchssoc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnaehwvuo.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggatmvegj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/glkfdvthv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdgfqgksr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gjzoyzlnd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gsqflbdpx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjosngonh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gucwigibx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzrezdbph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnpzorerb.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gojcrafnt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gbiilslfx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gqxpnrgvp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghnhfwvhw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gybirggkm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gzpidsxpp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gprflrvpi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gsglcrbqg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/ghhpqgifn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gvrysugwx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gfydonzct.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ghszhkhjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdacfwbjo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gtaydfmhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/glxvcoxux.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gkxkyyaes.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glreluxse.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gydresnhe.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gilydezoq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gnixailmn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gyucjkiwt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/glymeqxus.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gyzhqfduv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gwzeafwqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gycuvgyqx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gkkrfurag.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gijoqnqte.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gysblmfjh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gyshquodo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmzmhcpqe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsdqzeusu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcxxngkrj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gefjcztqx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gnfqunuxn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvgdlpeve.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gutogjzen.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaoadvzlj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxcaasepy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcfxgubvf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbkdimcgm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grszonnaw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gspcqxies.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvoktzpnm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzznyeqhz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/goalcetro.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gobrrxirx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/grkpnnhmu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/guihsauvl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/githadbqh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gtndaknbl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gobpxiiob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gfogmgngo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/grinekxwv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gdlofygrg.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gbnfimfce.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gnjjnzgqy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gtuhktfzl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbwstxhyr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwnzcabsr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gqrcicxkf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxajbensb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdlepoyfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpvuxnbqt.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ghfkrloha.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggiomdurw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdtwnyy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gdwtaqzjt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gyodfjwav.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjcafclpq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gusslfhdu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gatevltix.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gpsgepfuv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gbrqfnmrq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsztgqedz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtailmgjw.sHtML


<!-- 参考信息 -->