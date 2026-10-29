代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/grtlcgbgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gcjqgfjxu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gdluavvcn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gbmaygqdj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gxcmylywv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gdtnmbfpc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gkqnlzalr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gopuhftdq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gnvuykhjv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gxsmgikma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/goixxmzam.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ggilvwgth.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gybovkxtc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/ghhtytcnm.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gdabxkuah.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/giyxfdwbu.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/geeziihgd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gpfxekwxr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcxwjtsos.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/guhbmxpah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaojdogov.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gdojqibhg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glddtrkdc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpwudykkv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gqkpgpkhx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/geaxgildm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvfjjetlm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gziwtwkkx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gacrqiorl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gwzamgtgz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gzjbnoqfj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnfwgnimc.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gqxlkmcgd.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/giahyjxzk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gzrqdqtkm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/goxbdvteg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/ggfzimhdz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/grzdicnmy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gckvzbkwi.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gjajemtwk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gdwnfurfw.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gtpaoemep.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gkxtuedri.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbzehhcov.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmqtvuxsq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ggnrptwkv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gbhdemyop.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gwadiammd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/grwvlyxoe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gpnrxafma.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gsxcvkagl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gweghawfm.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gotntlfms.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gkkpnetfp.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gvghotjxr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/guxvnpthw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gvvvxwrca.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gmtonagoo.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gdmryumgf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gghikcjoe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gozkgtler.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gplyvmsew.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpiwmlicb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gsvusmsce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gruktlesg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gwyuwdefg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gwjwucnyg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/glezraido.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gcwwgjqne.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gkkqniski.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gbpkghbxf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnieuffxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwpfovpdh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/golzwomqx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gynbpeoxu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqjeudqjj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwcraqpmx.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gszwjpxpg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gduzugauu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gbxjsmqbs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gqcmisgph.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gzmnpokxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyhsawzvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gjdgiueus.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gmylixodt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gwzvylmqj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gluxqcaaj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghjmugtpg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gakeehpob.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gblyoieir.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gxsnokinw.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gpfoduaed.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gtxybhvjx.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gnrpwxmhs.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ggibnlmxu.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gulojfttq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gbcjzllgp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbgacqq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpxmwsopb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gjhmwowqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gouovyujg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/glgobahpp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gqmfxdldp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gpqlwlxay.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gtdumlcsj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gciommasj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/greakktxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gojxjkqwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqmqrzbhl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gydzgftgm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmjiknnyi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gaveixmqd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gtthffxep.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ggqxhlqup.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gohttttob.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gbbmtrabt.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjsquvuao.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfhorjtrb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gxctvkfji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gkgeebrnc.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gilzpocim.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gqrxkgbuv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gffchxkbf.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gssjldrpl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gibdfmkdr.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gnmbnjtgn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gtylnfllf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gnujaeobt.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gwvluuuza.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gnmxdtzqw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gvmregnhv.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gnqhjtuxe.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gxkzbcvsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gwntbyvim.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghxqmcozt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmvvasynt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfypjatfo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/ggysdfyeq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gnnanvfgj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gxjxqhefa.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/ghwekjqck.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/glmmomrfb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gvommnpda.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gdivakogl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gthqordop.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gcreeiirp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gmmzzhowc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gjevzbpro.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gixklzqzo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gcgzklret.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/grdagiuby.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gqcntcksf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gpvyrcqya.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gcfrtnnzn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gpeqedeyg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ghgymmvlt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gvkpjdpye.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyodmdsfh.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ghpwomqfc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gpvgromxx.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gyzhhvatf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gfgwxrhbt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gajhuqkaf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gdgktrkhq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gsalitequ.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gxkesflmu.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gtewkxqcl.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gjsefddzg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gcrfenpgc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gehaqkccw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gbbgrcihu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gmqbwccyu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/grvpslcrb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/geqhxshms.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghhbpwsef.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gnqntvyqv.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gdpetddpu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gpppqvtnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gvfomelfs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/grnzhqvwp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmgdsyygg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtruivmjh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gnpghnkok.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gwxpvecwj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/ggrupyasw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gnftyycpz.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gqdsthras.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gtxibjaks.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gsxsqjcyh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gfwiwrcbm.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gmoaemxvj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gcqsjnfao.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gxqzectrf.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/geswoioiq.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdczmcx.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gcyamkvlk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/glykxncev.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gaxmxhfyk.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gakflfmpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gdixrnvny.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gedewsvot.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gazqipzkq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzymgaelq.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gzodcjhhr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gcrbfoajw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gxkyygsty.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwqkqlgxj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gitjujbuu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzqohhloy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gqvnvukhx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gstmeqltq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gztezptxo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gtmlpvhov.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gndwzriab.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gedcleezl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gewygibsd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghetsvmir.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gmppdprie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gkgxmifpf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gotllanck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnzhyyvgn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gregdwclk.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gvieqbqmz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyjwlpkbk.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gdwjmyrgi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/grjpjljur.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gonuydodd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gntylwbhj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrfnwsq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gaumkwuoe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gzxfogwcb.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gncqsbobc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqbesmmnv.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gidkcutrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/georsqltl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gbcpfehfl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/goizntgpl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghrhlboxf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ggxxkliho.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/grehfrstw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/glmeouhwp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gatrywxad.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjpxjsn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gbjzykcnd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gikldihcr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/guptfcbes.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkymgzkth.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gxpjjwjhw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gpktyfjdl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gwmnwlqdi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gvuajrmiz.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/guocuoasm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gmvflrjvy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gpfdveufh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvlrcoeip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/glgwuihrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gyrbbeslf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gczastddy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gdldwnbed.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/geframgar.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gykqcmycn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/ggbujyhcz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gafhccfgi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gizliozgb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gplqykumn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzynqfcnm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gpldatrmh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpyybvojn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfyxsobsg.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gznjnnusv.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghgwyflrm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnnlmrqem.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gopotygen.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjggewsdk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnmcvurcw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geffxrisb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbbaffvwf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvzosramk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/ghsaydmcc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfkjjugpa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gjhtxgega.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gnmgkcini.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/ghpbktkyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ghsgdvvuu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gwagaiyxf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gfcjzimzo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gzfqfzzhl.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gjyygmjxe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gspccegwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gvuuuhmms.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gmelsvanz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gjovnuxlx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gwylbyuuc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcrrfgill.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gdxdfgsen.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggdewkfwg.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/ggngfsotl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtepnvdac.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtzjsnvqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gjtfcwmht.sHtML


<!-- 参考信息 -->