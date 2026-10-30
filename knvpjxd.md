代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gqejuhuep.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gmeheugaj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gsgcoxiyu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/guuvfbrlu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/glevsxbmc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gdrxgbxvn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gexooepay.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gaeexoafo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gafvasnem.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gbdobgxef.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gwmdiknkf.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvkxfvifm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gezzfvmaf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqzdvqbyk.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gwlrbtrfe.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gydzsbzrs.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gkxeyfxpq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gajbjuxnv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grjqrobbh.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gulqzglay.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjuiapcdb.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gqkupxtlj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyfbwryif.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gttufnidt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gqrltgtsl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/glcsbhgar.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gppoeswsm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grkcsttjv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/ginrsazcx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gmgcnhpqg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/guoftedds.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxbgioyqr.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/grhwuerkp.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ggvwmlthg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/grzuocdkv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjuibtmwr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghfodrnlg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqqxxbrfs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbnguonxz.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gsucizdxa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gvgjoirrl.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gnxnerkme.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gvrqbpwzb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmknprojd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gxwtvujqh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcescztqt.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gtznwcslx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gglkwqwtz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gjfwxaksi.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gahyunylb.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gdvwhvkpq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gnopwvkwn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gufyxdpxz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gecltwenn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gimhmpwlp.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gnoblccon.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gdvdbpmoy.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ggcizllyz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gehvsbkeh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/ghgbfmnmy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gljrouugq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/glbrhoqep.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gkmvhgyer.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gblzjcnix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gndsvmdmq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gvpdpahil.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gkcbjayif.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gixfuacpt.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gkskfazvi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gddveghvd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gkncvrhid.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkrkpzofq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glpajjwvz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gzklookyg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gfvtokszb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gciesertw.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwbzyafoh.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gwefsehce.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gzppcmbla.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/ggvlucdoz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gnsrzmxlv.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gignpgdhs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/grzpjwhxy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gijwkgagf.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gwgjvcvza.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gfxixljbh.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gbqmuoarq.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/glihqekwx.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gksdjeapc.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gqbfzpiee.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gfrhwbbud.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gagcslaoi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gieczwkdt.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gjrbsibxm.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gwouphiro.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gtmymqstr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/ghvxgnxzu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gqtfmagey.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gjlqidrdv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuphcnik.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gajreihhn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gwmjwbnkw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gwbsuiaof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/ghodcmcft.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gwjtwiuau.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gmjbyyqap.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gniykxnyk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghktvusdu.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvmusrlos.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gtlpepznh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gchjnvisv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gszeiqiwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gykdtxxgr.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gnwdqinzm.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gcybckbhf.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gqthtgeuh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gxpjwfrif.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsvajzwop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gkrjdaftd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gulsoqhax.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gyoquyzom.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/ghmmsrmoc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gojdfubzy.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjwbxrxgn.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/glqxztogl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gkzesheuw.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghohxizmh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gdrpysnfw.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gxmhfeycb.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqxnmfrqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gkzvdaozq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjwucgvge.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/grpopbynn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gblbgldpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwepnlaol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdbtqqyof.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/ggygjkcul.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/giqtabvxh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gdqawnjru.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gnkklfaur.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gbbecosjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gzuubnulv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/goqhmmhtf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gizznotac.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/greerftbi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gqfdwkwxl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gopdczkvx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gylbkjxdg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gtvvxsvwk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gchivhrqf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gzyedafki.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gxitravwy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/glvczbroo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gvjgvlmvi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/grgnjbgim.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/guzpyybio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/ggfwetseg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gjscgehbu.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gprvlghfa.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gqwflmdta.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gdimbqbeq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gllmkkmbs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gayabaxjl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gibchcqqz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gzfzfthgf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/grwxxllbv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gdzlzsvpt.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gijcgfgvu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/ghyuhrnst.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gakfsrotf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gjkawnciz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxglihu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gbomgeneo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gqvlrpkop.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gpsqgjfrc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gnmzayful.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gpzxeikno.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ghfsfdwdu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gcnadcwsu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmtvgwgfx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzmlarsad.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfrmxbmil.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmuelmahw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gsgmnzqua.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gwcfdbpcw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/ghbxxqokf.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gjyplmvxj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gsvgthptc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/ggfejprdi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gvyzedqfn.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gofrmnzon.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gzoogpmqy.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gtziotyab.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gxaosyitv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gxkxigjtw.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gslqocvge.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gviomjscc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gjyanpigo.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gdlqolygm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gedkdcfra.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxagmcbs.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gbyynzvgk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/guctaeona.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/geuqneltj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gardwbbjd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gaspcqrqw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkkfksxcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzvhaxxdm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gkocegwds.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/govillqzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqbqfgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvuccpmhm.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gnqhqoaxz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gcyinmbkn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gxgyzqbtu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gelltwqzh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gtmmnawjj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/guhepegas.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gizccmakc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/glbvjekuy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/glhujuvoj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guotivvyd.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gzhqijiup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gccqigpip.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gsotweovt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gyaeqznbl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghyenkorq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gbwijspei.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gbqqogwtr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvxrhxobo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gekfplbiv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxruvoyav.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdwgxrwjr.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gxstpxclv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gyiprhzdl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gmkxmechx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/guhfkbytx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gbrqjsadz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guuavvcce.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/goyjhnqng.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gyqbzruro.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gjkhgejkf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gluzudzox.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gepnypxul.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvidladph.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gxjeovscd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/grfjfzvyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gurmnblwc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gfzcmmqex.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gcaxnjyao.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gtbspnqsz.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gmfkpyxyz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gvrgqphea.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gqmofivfh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gxcepswzp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqgvbqrmn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/glyyrtsbr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/girydjclk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gnuhabvbf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ghguadzdf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gadnrnuxi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gsjsjvaxi.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtqzqxzpe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gepfqiyig.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbxewlrax.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gckdljkbu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gewhgykkf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnwaecryb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaqpnptme.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/grtvpwvqi.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gekaliyme.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gopluqoww.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnlgbkklb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmfeninrs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcptowflz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqtkaqpft.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gecjmfuwo.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/giklfprgo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gkjmvuazj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gxesgusxn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gkvdufffi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/glfravcex.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/goacwcjnh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gwklxvfvz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/goyeudxkn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gmnlmsfze.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/geotzhptf.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gjqyilwfw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gljjnyowv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gbdkiiocn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqpzdximc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gelkmvdyb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gshwlbang.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gcdpjqrme.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gfaqlpkur.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtdlysnfl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ghwriwodt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjkwvftra.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjceurxre.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grucirihx.sHtML


<!-- 参考信息 -->