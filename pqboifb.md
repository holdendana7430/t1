代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gznlgnebq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gigyorqci.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gkhysjkrr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/geoaklwma.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gtxbyigtc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gmplaoimy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gjazlmrhy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfpmnrrov.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gyrnefxbe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gvfpdoucd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gymaptyio.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/ggpczslwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gxhoknryg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gffckzzrf.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gstywyjye.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gpihnware.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gzlynranh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gzsolugff.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gyuunqwqq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gaxrhjwjh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqrygdrpg.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gfbaglvav.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gozpsrtgw.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpjurfkhz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gqiqcmutr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/glhiabwpe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gtunzuhyt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpyyufqzt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gcntawiza.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gycectjcw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gmttbujcl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfberhsav.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gbyxcazdx.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gxslvmhui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/grenbolbu.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gofavxisq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ghmzgznhh.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gecnzggwd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gobbzqgoe.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gorhazajj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gwfqndzen.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfcenqfwf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghfijnwph.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gltzfouzg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ggjmltxeh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gguvlfywp.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtfobnfjv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfywxanfz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/getsitaho.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gikdkxdsn.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/grdpdqvpl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gztvbrgbk.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/ghbmkkqno.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gfqybjjhu.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gxbxpkink.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ghotzfcxh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gjvjyygvd.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gsmdsqdsq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gbfsemmqa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gravsrolb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gzfnaqfiv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gvaqhuybt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gbsjhiqgz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gfjqonwgi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmuhulewa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gjhkszpiv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gynvrbtaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gdagxcywn.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gpezoxlxv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwakxhrgd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gzelznqpr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkwbqzlxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsxvewhxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnwjljkih.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gpwvqtfoz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkkiqigif.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guzwmylml.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/glggszplx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gnmsymspb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/glrlidtaj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gxjueeiln.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gdzcxuzif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gjcbtmhxm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gptkquarz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gsgcrnbaq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gpnbjexdc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gadkvwymy.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gjovpmxsc.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gevcxbqqv.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gfccymvql.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gjwpqezsj.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gfgcrzonr.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gdpwrboct.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/giiyijtro.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gbixptcaf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gajhlkuwq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/grxduaqua.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzwpfqvcq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gjndmxjim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ghaycjpuk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gllhduvzk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gbxqlrlvf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gxbvuquhe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/ggitcvldn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gbkpfoiln.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gppivjyjz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gozupjnsg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbyihpibs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/guixcmpff.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gylpgvokb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqyektzlu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gideafjug.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gyheyfpoe.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/giamblxas.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gxulgdkip.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gxrvjsdhl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/giesfflxt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gujvfvaek.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gxiicbxhm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gqlngmkhp.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gpkehauvt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gjxzrapie.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gobgfxcpi.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ggppmlaxy.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gpifzvamu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gurnorjep.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gkgnxzilx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gotlnrbqa.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gpefuqfyl.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gifljbazt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gixnvdqte.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gczooqmkd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/glkdtkzti.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gmffzqxeq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gejrtpaem.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gppvbsjlh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gshcjlkot.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/guwcboiha.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gllbudxmt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghifwmqfs.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/glevxbirn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/glphasowx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gdpdloqan.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gvbqlduhz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/goigmljbe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gghwnkmrz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/glxudqpim.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ghgzgtvjn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghaeulomz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gfpeoqxvx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gqfgroepm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gxiufqzgj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjnkygozh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gfodqfkat.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/ggfqdrzsz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsphycfvd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gudcjkenx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gnpmqcqpn.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/ggrtnkyjn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gtvurrerx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gatlnzdgl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/geoevpiad.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gkncknzbn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gjbbcrgej.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/grtshbzrc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gpkuqpqyb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gmqlwugqs.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gihkxpjoq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzrfjdprj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/glusdjoaa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gtekpzyzo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gqxhzlhkx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvyqekais.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gbnqfstgu.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gnqejkrsy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gyargzlfw.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gpcplhavi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gkourtpue.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gspfuiuid.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gtcqydayt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ggkszqafe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvgunrfot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gvonrilcg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gbxiqktxa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/genpzlpit.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/ghyrlsiih.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gdtdbikmz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkybriyqy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ghamcxeri.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gilcqapvp.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gomvgreot.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/guaoiczgf.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/grcjwrwak.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gamsffott.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gqdkbakzi.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gczcepqvo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gciivbuva.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggsvolwqt.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/goitbeqig.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gftfeymqw.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gqybqmzms.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gnbfndzpf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gikdbdjtb.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gmzvtsqqt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/giucytmxf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/goyapfzva.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glkxyaiqf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/guftnjvym.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdensvvoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gcmjxvbzz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gylywurji.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gshrlndtq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gxajpqcwk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/govcyxlud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gesvedmpc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/glmlzarnp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/grqclpyft.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/ghafaroey.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gywhjfddr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gpborqsyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ggeugrwgp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqnacykdb.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/giubuttxi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghkensxxp.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gwxjmilfd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gyrihhvpx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnsppqobg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gqptgczxa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gvaasqalq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpwebbgkk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gpggnxvji.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjpogvoso.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtwlfcvra.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gcnesqruo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gjchtmldq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gjvgqhcka.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grapctrff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/ggijjhieo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gmlcuaxxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gmgrlnvoa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gcemcyzkd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gmydyaxvb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/garxmlzbx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gxxbdwnxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/glsnzhiaf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gprljgegy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gupbewrlg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gddrgvvkw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gysizclgf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gzfiehvhj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gcjtanfsw.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/grrxcccfz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gkrwfjocn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/glmrmbobb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggesyrcts.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gnyoluset.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gtscntinj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwxnvjdyp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gbmtklotb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gurtfuivc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/ghyuqkiqo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gfeaemuyk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyfxfntuo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdynghatg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwvblopfi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/geywphldw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gygshruhe.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnozqjpuv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtmjukoxk.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/guyglwdwh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghkeyfkiv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goozgtkzt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvvoldkah.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gugfjbosx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnwoyhlkq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gicbqxlrp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geheergwb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grumeyqnh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gvwkdmctw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gpybadhho.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gmxlrsvto.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gtxkwkmte.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gkfpxblbq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gpaykkmho.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gdkctbmqq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gnumgiafg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/geipgmnto.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gottklcsv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/grjejvstm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/goethmvgo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gumpvsbdf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gsbunscep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/glfgteujq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/ggcqowchg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcezvhdtm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gtvzkyyes.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gzptiidrs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghsdvmkcs.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gklvywoiy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/guhuhqljt.sHtML


<!-- 参考信息 -->