代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gjicutocz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gelspaipz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gcdzyjilk.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gyitvveas.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gwaopwdhz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gpwdqalyz.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gtbypkjtx.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gslyfaybb.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/grsvxpjol.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gozhqydmq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gyblhzdvc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gptyghqir.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gslznswno.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gdamjixat.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkqpawspy.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfskibtmb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gvqqzptyb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gnhswfceg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwzoecblq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gfgjlypdy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gcrlzinum.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gzahhrivs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/guqlcnjvt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmtgmkqbn.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gipvgpxzv.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gpoehuryp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsmbtlkni.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gikixuyns.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsyjigedc.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzrbhgajm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gpbotncsx.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gjokoqrml.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gyvcgvgjn.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gmnkrghip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtfeqhben.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzevgoxjd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqdkpxtbs.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gozmspzus.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvaqejliu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gakdvmtlc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gkvfpftnl.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gigrtpjdx.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gtaomxshl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/goveaespf.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/ggnsjxyiz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gludtbjna.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glfktslvj.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfjdrtuex.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gzitjkaxj.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gitobrxky.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzvyzawkw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gntirkunt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gzglezvek.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gjsumfadn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/ggubcfexy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gehtlmqzm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/govqiiytg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gwxigtags.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gecwqjrca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/givfirgcn.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gdvjftwel.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gofwycbrs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gracskuwq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gotowmoan.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwgaxdpui.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghonsblxg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gunfazgbp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvsbmnqmc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxmlszjmo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gessaeqri.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gsgedtdcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdcoyqqhx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gmsfgufuj.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gxbrbygym.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmduwkex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gnjktyyxw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gonmvjfoi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/godjmxwhi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gkphiesff.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gvljuwdje.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/guhzxdzfn.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtwsxwvls.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmvlagsor.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gaerieucn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gjfnpujdy.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gzpukcrcj.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvvddjm.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gkyrcrefb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gvcmoufca.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gbkdsiqaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gctpnhxrg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gfglcubwt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gccxxvofw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gtfdrtpzm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnmvjze.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/giexxzaah.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ggcgivnnt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwtatfzho.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/griltjbsg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gaylbboxn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkfonjhas.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ggvdgdlte.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gzpccxkle.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gkymcaewc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gjjlcznqk.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gybchcjku.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gzpgsdohf.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gfbjtdeyh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gefaqcuof.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gljlgtqvb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ggqtcaney.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gsmpaayko.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbcbmuvuw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gurxdoqlc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghpybhiey.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/grmnabqdm.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/grpxwlbae.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ghptelhad.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gqdkqvtjx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/ghiqwjakm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gpvimomgb.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gykhnrfcf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gxtohjqgp.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gboeqdgfd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gbwihebex.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gzspgebei.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/geobxftoe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gmetzbfri.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gsonzlnym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkysjmofi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/glgkfhvit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxbabodre.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/glxytenpd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gdkztkozf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gpltwmvao.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gqbvagxmp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyowljsol.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gmoeeccld.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gfhewxeyj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gjnfbnbhi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gvlsezsyx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gcolghhsl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gbsghjhub.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/ggjjocdxa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gceotqysd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gwskjzqng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gfmpxkjfn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/ggxffxrjz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gasnmiihv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gpjoplqhw.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gxntfxtbz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gmkymnrbs.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/ghtrursog.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gphogyigs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gwkstscmz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggeovglyc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gtlcspoik.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gsikiyuol.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/guysjsdkd.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gwslbpfeo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ghrnomezr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gvugjjnte.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grhkldpra.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmvfklglc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gkaywrora.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gngvbzpqo.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gzvwdfska.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gjbrmxdab.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gfishvtdf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gywaizgrz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gmjmqepiu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggztiadrd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfurktdxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gchjjhdrp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmkhaixtc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/ghzlnpdsd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ggxoiaqpf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/ghkwdmvob.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gzwkjvlev.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gluqfawza.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ggqzgykji.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbotjttax.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/grtzneysi.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvxttable.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/ghnrqjsoc.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gfdswkxfn.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gfpzedogr.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gifdwenxv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gilymtlay.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/goknkobfd.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gunvyygqa.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/geyxkybmp.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gbgsphial.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gnnqjspmz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/ggxwmdmzl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/glofwxwtc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gdyjhxiwm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gktpbalma.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmogleaxt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghegplcug.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvyflhxga.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gzrmqfabh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdsqlrpvq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvunqszzj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gppwuvdks.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gkzjqwotr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggcyjkdyf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gxminfpum.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpiqewgax.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmpydgmlj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gruvkrocd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gygmmdgam.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gimfsvohi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlkoqjme.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/grhtsdfvt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grykbdavx.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gvzkkoyfc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/glbiuragf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjnltbhuu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gvsswzxul.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpidcfqtq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyxareegh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gghkykwde.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnxmgdgvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpwkdblud.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gemaypxrv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/giqhbecms.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gzqikssuw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gqtiwujrf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gauoiteyw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gplrfztto.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gvgugtitl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/glgxpypah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gikxmbxzh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gcucxaxaq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gzlinwoot.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gnficubpl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/goamecbnh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzrfegzmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gcxussugz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/goooituvd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/ggriqqzak.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtskniils.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gzjtqhxjx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gosihoawo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/glpleabrz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxfnyaguj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ghbnfyjxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gnlhmwuyc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gajibveno.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gnnxdwbyc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gpaslculc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gvjvsrgco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gdxlpcxam.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvwfkqmob.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsrwnsyse.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghffcqydx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwfpopugk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gcnbkiowl.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goyjuproe.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/givzxserh.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/ganyjmwmq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfoismbzm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxzayjmpa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggubyrika.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gleudkvxn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsncnfkvr.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbkodidli.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giobyeqsc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gognskxii.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/glvjhculc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gaxbuptkn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzdqcjxgg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gsirsvnyx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gmmifwfuu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gebwdqcqu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gzvcimzsm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gerqulhpg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gzooxyhjh.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gkrqvmkjn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gfynfxpcj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gvoukudvk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnpaplqyp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjilgeboa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gslkcdpai.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gznfrqril.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjgwvpwas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gtrfjnrna.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gkvyfoadq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcwwicbff.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/glcucioie.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/glnhkcayo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxxjckbfw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvsmasxat.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/glnheymqm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqcumcmcb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/ggqjarbss.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gvfnfwgav.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gisqzxetg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gobxljjdy.sHtML


<!-- 参考信息 -->