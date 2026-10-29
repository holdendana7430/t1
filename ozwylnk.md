代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/goctgjdhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/givcpwglt.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/giehvdxjk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gnlwijsbg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gcpeiwoug.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvekrrzvc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gulmtpguk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gapdzqtxe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gvokxgvuo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gcldahzcr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gyekhpyfl.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gcxtqrbqe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gleyrnqra.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gpzqkfuio.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gwoafrntp.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ggibfsrac.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gbvxsfxbb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gegmjvvqx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gbnvlmyeb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gsjbknnja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjrctjblr.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/guyishqhf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gejayxvkl.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gliqcficq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gxdrmdygk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/giagpmbxb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gpasugybm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gwbgyswvv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/grndqdhan.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gygbecenx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gitajhast.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsvltxnxy.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gvqndszkr.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gdffpzspl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gkcrxzmmo.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnxpzjpct.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gkisckiww.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghbnqeiwj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/ghkbqtnsd.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/giygwvsis.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gadryofdf.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ghyphfqhl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/giomgelxg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gcqvrcrcp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gtacifmjz.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gcxluxoln.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gqinhmzvm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gzfnoxzum.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gadwccvcj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/ggyzmmkpf.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gxnxxiztc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gaabexrwr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gsqyigitk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gluernvpp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gdvnvlbnk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gshmmlhoi.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gpbolxyqf.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gbubgqweq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gelemqrhx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gtaanltrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmllbxzvr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gacnqtqff.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gyckbcpvo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/goprysrwb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gscblqerf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gyoufxomk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gujxdxozh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gemtftwdn.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/guscklnii.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gpyffiruv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gsfrlqpac.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcvrppaxn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdhkrvlva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghexjjjus.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gyhfcpuce.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdkzsmvdr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gahjqptzn.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/ggbrbusep.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gicirjzrp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glunoxflw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gfxymkqdb.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/ghxywpovi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdybdaglw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfxjrqais.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gobaeoeih.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gcdhvzfwp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gcqchkbyi.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/grkeetawd.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/guizvmlgi.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsddlhprq.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gqnbkyyss.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gdfxfupul.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gpucpximd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnthbfb.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gqiaxxdda.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gzfgudbtu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gbufhrrnl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/ghjqoqahv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gsnnlyvrq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyamzkgcu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gruphtwry.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gderbzihi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/ggwdcnehi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gpgxdrxsy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gcbmihjee.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gclcnydbx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/ggohomvcd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gqzfyhgvj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gkbowktlj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gjkhtdlxw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gahomodap.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/goqblyxdz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gopteqink.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/grtxzgjvk.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/glxgikjzo.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gmiiwajlr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjjiueagf.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggnzaizbe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqqlpdbil.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gnyevford.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjcexawcv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxsxmukuh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gyfjdmruh.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gpszpgngc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/giawfndzy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gbtcthiko.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/ggptxtvqi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gxfftzokv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gfrnywdsb.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gqkchyjnc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gxxouxdou.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gjaezvfii.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gefzazcbp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gfyletfqy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gujeevwum.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfnceccdy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gpozpnvsx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gytxpcocx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gzhkmmucy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/glfkjaama.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gtnrrspcs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gjvwzwhis.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gfsgeuoxn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtsgyfmqp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gysofgooe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnaeqljso.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gmzmplipo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gwodvbupt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbinmzfye.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gzjjhewka.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/ghmblpuok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gmbvzeywv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gtmvglumm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gwfuqmmrp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gmnbguyzr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gzmdcwrxr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gbsyrpssb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gletqpojp.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gupkptkxs.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gjdlaljts.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ggmudhizj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gwatwfcnf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gfqxwrauj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/genjhxgar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/grcpguuwi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gxmoruduo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhwvnltp.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gaklaaiui.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gllmrosnd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/geaarefsl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvursgmen.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gcpxemkst.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gbypcutjg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gguxfmbtu.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gdjzugfke.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gazgnqmuy.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/ggjyfoaus.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gnzjzvwzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gwjrabzes.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkrlybeav.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggyhszulw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyokaxmtn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjnpjfgrz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gvcvbkrcj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ghirdsrpa.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gxdyrasga.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gccigpelg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gcypomdrb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/guubakxjv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gvsfnjwox.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gvzvfpnlf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/goyabwnwo.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gcaznpaub.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gvudxpzne.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gcammtcgd.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gmhwlcxgw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gehajrqgk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gxknpefxn.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gccuourat.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gpynddore.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/geobqpcej.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjfcyao.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gphfpqjum.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gtmbcaamx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gnzxmxdux.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvlmgscvs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/grorbtgye.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gsztqdldv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjuieedzd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gshsuudob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkalfcaqy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/grumzmttm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gfugelopf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gsxszdyqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/goehksxxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gjfckejqg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gmnyjqukj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gmjetbahc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/goicxzacx.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/grppgeriy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gmjogaxrf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggnvuuanm.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gyjvbarcr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbjggatzx.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gchuvcxzc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gmqelwfig.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/giicrbkwd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gnzdqjjlb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/glrhlhmxb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpeipgwso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gjeirkrcu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwouzauqe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnspfdqzd.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gdgohufmv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/guieqymra.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/giqksqgtd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlveces.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gdpasewaa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpssbullj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gvzyxqfbh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gnvkpyzue.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gupkxiktb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gtssztyot.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gqbvofgrl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gautljroq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtohrddqn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ggejbcfyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gglkcfvxw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/grtxpcppc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gxhpiufql.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gwakspkbu.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gmvbrzvbj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gildnbpuw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gdahoedvb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gufwypyvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfiaqiehr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gtkmgaopt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gnngskget.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/guyywmche.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/glpoezifs.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyvocvils.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gpomdijww.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gndyxzbdn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghobgvaqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwdzvulpg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gppwemouf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gnbrfktqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gilesjfhj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfllkcvgj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjueiri.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvhajhons.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjcowxnfg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gydhgbskp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsulfqsbq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gsqzvlnsd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggxxlnnny.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjtzfljmw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxwvimyvn.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gsachlyyh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqroesnny.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/geiirldot.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnalwwsua.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gpmjkuoto.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gdvxrfxdv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gznarydcu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/ggepyyoyb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gtjkmqtsf.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gmlvkxpsw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gorjejkhl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gdiukkxih.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gigrolbkn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbdsdmomp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gmvvlxzfk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnwqvfuyo.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/geuupogxv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdwaaynyy.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gkciiambd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guljeoaxf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsspwwfwf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/geixgcxae.sHtML


<!-- 参考信息 -->