代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzgsvuzxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gbvrpgywa.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gzqfxgopg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gaqakpenj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gofmwlddf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gdhqncbgp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gyclhafbl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gfffptisw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gxgdltxup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gupcnkerf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gcrinrhwq.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/glvlmrnfn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gfnyjjbkr.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/glmttjdzk.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gphmastni.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/goedvbbmp.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gxcjafabv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gjkkdpeof.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gdznuywex.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbyoylvqn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxwimooro.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gofwqqmqv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwmwwjjmd.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gzzrgtxev.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gevyxrwgi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gwsfufmwr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gaemwyosu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gigykcaev.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gmrucfzyl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gjceimobn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/getfkjbcz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghsiwdjdc.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/ggyglyiou.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/grdcuxglk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gxywxagjs.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/guydqkcsp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/glhzqiqoi.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gernbtkpq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gxoovbpbn.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gahliqqvh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gsglkdlqg.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gpwywqksc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gnqcluzwx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnmzmnojv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gxtqyyvmg.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gafjbzmok.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gwcnumjge.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gxatfwqju.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gtuxjmdkw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/ghekijhmy.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gozncfsdd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/germwnaij.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gyjhtcklz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gazhkaaqy.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gqbzdsybh.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdbbknusc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gxdtspsxv.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gbdzvoigk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gukxsoukd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/graxglchp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gzsiqisrq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gcvascprw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gpsnqfapv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gufufbbeb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gltiebrmy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/grlruhuos.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/glflcviyo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gowqjmyzc.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/ghyjcyfai.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gvylgxihd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gtdkjopjt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gawazrqdd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvxcnfaad.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gawxeokfn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gxbopbcbw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gclnqqbgt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjfjncqwt.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/ghqhhrihe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/godgosoln.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggcqvtwad.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gmutxlylk.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gpppdruow.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glcvkgzbh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gngngcctf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gwyxrcfzh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/ghnvavjvd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gozkbbgeq.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gtjwzoikh.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gferljiwv.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzylpddbx.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjxufvohb.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gtauvhqdw.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gmdwhvoil.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/garwandug.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/garojxkzb.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/glyochels.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gxumpbtzm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gjnwtsosk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gwygburdt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gyjakdmrd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gwacyvdsu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gwlqwpfdu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpqaavjfs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/geoynznco.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gmxrfylyh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/ggrzhluwd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gfklhafpc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwbezkuut.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ggfasshdk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gcwakczoq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxpoyolfr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gdhnliely.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gdcnwsjwi.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzaknbfle.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gmufdutmb.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/ggzoelebh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjbbvownn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/geqfrtgqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/genrsdpug.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gqktfgieg.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvksnwqwd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gjxkjzrpm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gqrlsexio.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gccwqxfap.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/graebnhxk.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gfzsdzbqm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gyxiufjwl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gfknxefig.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gtonozjxp.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gudeabueg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gqmbzdfjh.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gekbajhfc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gcmzpcmkv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwaofvmgp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/guouhwjvu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gvksczqey.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gkzvknriy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/geedaarvg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/giqindfik.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guvtiybky.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gnkgcotny.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gdwltmczh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gukcfbsng.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gttjuagcb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcmwmacov.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfwgsxnf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gvejfjpfc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gbdcoemml.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gyfgguzcn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gpbjgcxjt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gjvqrnyrb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gfmutzmod.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqvtluxps.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gfjsicgvu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/glpdmtfck.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gwpnnqpyk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gscwcuyxj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gokgbckiz.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gjdpmjrkp.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gunqfzhrs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/ggdamvuge.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gmtbjtfap.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gnhbbuvyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gioukshbm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gwumssyxk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gemvikjmr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/geelvkkzi.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gbwsevwdo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/glyfuelal.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gziolqxfd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gnlbejcur.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/guwhssjge.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gytfdyxue.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gupjmoupr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvtojby.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gvldhildo.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gdifjiudg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gsmckzxpe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gsbipwyuq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gknszwscr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfcpqsmaa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzerdclgm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwaykaket.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/giyjitule.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gqulfjhtf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gkdvtcvjp.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gaoqqszrs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfcwxfuen.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gkrmbjhky.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gtmxzajag.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gjrqlgojc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/ghpopbthw.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gffckfmyj.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gaxgfdedl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/ggoclugrp.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gslvwkezj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gowybnxug.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gjdkqgmvx.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gohovyyxb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gvpwufadn.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gwuvypqsq.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gpmhqlhrv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gxfrqmaoa.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/glwdetprx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/ghzrllulq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjzcigxnn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyxhlaoki.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdcbqnwnb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gaiyuvoum.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gjeykzkoq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvutlxroo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grgjtnswe.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gfwgzvpqm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ggvkqdmlf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzwanecgz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gllaxspok.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glsqktmyy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gsvvskkns.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gdqaksmuk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gujsphbki.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/geihvrgjk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwkoyeltb.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gviznzfkn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtohbytkl.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/grujniawx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gksknqjud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gahydlamv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gtwxkvhbb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/glpdsbgwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/geuwgfqnp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/ghcqzjzfj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjwyittzf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnhdgvetg.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gipyleowk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gpddppcte.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gfalhbbmo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gkwdfxumc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/goxvltybx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gdqinpjti.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gnlkzocnu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gttpamyto.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gaqsqpdiz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gevymrslc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gkbmkgxtc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gputwlxlu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gbjyioxit.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gszbrbiyg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gtmgaaqob.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gjfbjgyuz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gdzxiilqi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/greeguzsu.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gltdzdlgy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gshpqaxcu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gwtyxvoyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gwstgugfm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmirqevrr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/glirfkypw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gujobqlst.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gzbasychh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gjovfbjdv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ggvejzbxl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ghddpvmcc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gksertgpt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqgafwlgb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/givbtikoa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkduyqzjk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gxmapnyzn.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqhahfqqq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxxlhjszn.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gpizwlmkn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/getcuxwoj.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnwvnkorp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gngvslrzt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxbcrvzod.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gitadtfvr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goszzhgtf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gajcfpoez.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsvrcsujj.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/ghxnebvws.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gwjxejkdv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gztxxpsae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gymeuipnc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gqrdypkfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gqkzzwfip.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gxmgqkfor.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/goasnmeny.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/giwcbokqh.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gnlpcnrwg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gmvqatqwi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbmdpyyc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grsfcrrck.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/getrfmeje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gtrnxkbdo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gezuqzczx.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gxvauqvtt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/groldbryn.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gntcmobuj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvbmryxoj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsocjfyoy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gyudugulx.sHtML


<!-- 参考信息 -->