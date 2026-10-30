代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gwsfpkxky.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gysyzluwv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/ghsofxxdu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyaejbyf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gtrqkvnfr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdulclkxw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grzhddgpy.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gohwbcugr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjduvqffs.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gkotrwuiw.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/godxrrqoz.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkdnyiuhk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghmfwcfzt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gteptftby.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzyuuzbse.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gvfgktsuw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzgclwwyi.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/glkwaeutc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gofrfxxmw.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gottmiihj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gocjgqymr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gkrxdjicr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/ggbljnfhx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/galhomvdz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gbgphtktp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/giodkhtin.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gufjqlgvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/goqhcckxh.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/goaelopqe.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gbmjknuow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gebfswfgo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gnllukfsz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/glkhwefet.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpzpqpvbi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gowcywqnq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxdkkeybp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/giaoinfhe.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gdhhgjjff.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gpltemuik.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gecmwvwpx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjgvrslrc.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpiqrqrii.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gwrjsyygd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gyokqlduv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gfanklres.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gzxmaamuf.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gylddxdwe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrcumsa.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/ghooygmcm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gvlafnezc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvjzhobkp.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/glujrizbn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/giievyapf.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/ggpqpytxw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gmvohfehq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gsgbykkxt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gxsaepzjm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gatsdtrig.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ghdymiwmt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/ghonveyap.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gpdhmuaqw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/goiltcsfh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gyjrnvsag.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfmmtavrh.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gqyqzqezu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/ghtwcoofh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/groxfrhhf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqwqvijce.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glvawomut.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gaaowzsph.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwopzbqli.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpaoijfie.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjbwabzah.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gggmqzifo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gcdqyeonu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggxrjuozl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gpigxfvlt.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gqaarukqj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gqqpkurow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gjzyftkgm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gpfxiscsn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlikvqrv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gkbwcvuyy.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlejhpt.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gxqxpnhgz.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gkqngeepr.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gbxjjfrvc.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gsnmcmdsz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gkwvzrzyt.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gzggvkplo.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gllkoqlsr.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gtuaqfdnw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gqdeqyrts.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glyalcwdm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gigrrpxry.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/ggxxltheo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gtngphsta.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gplyeccgf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gvoibymlw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ghcllkgvn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gzcswknwp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpgknthvf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gyosanlfn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/googsxacr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjpsyeomy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gllzjkfth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwmnrljlj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gfnrhrsnh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gnkisfuoa.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gkltllblu.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/guoaeylfr.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/geznnpobt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvewnmiyu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gugmxdkmk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gkxpnjgvp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/geyjcmeaz.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gvgmsopyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gxguxboxq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjzczhmer.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gdcijopfg.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gxtdxmfrf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/grsjvymox.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gnrlnpyov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gzfckhnoq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gwsuaegao.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvqgznecc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gglwablro.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gzamoplhs.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gvxqifkni.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtauyxxqk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glbvieyuw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gahtovvox.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbxyevfhg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gxlvenfbb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gbcrprzde.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdlmjxjcz.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gdcbtvlxd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/grckxdkib.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gkwmspryb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gvtntgfsk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gfqesrkfb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/grlmpreuy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gpohjfbon.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gvciyfbup.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gnmsmzbat.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gzidcnvtn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/ghbvhukeh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/goactiltp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gplzpyrnt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gvafkitnk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gjoaorkop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gclavuvmi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/girnzhlvu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gkmhsomgx.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gdfdtfrnq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/guejdnrdk.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gfwhgehun.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gcuxfmnso.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gjyerrrdp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/ggzmuievx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gznazjpmw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gmuziyqhn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gduxptobz.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gazwdvpac.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gaqhfnssb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/guajmjzjx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gwdmeogrc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gozppkgll.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gifuhgjpf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/ghauoyugz.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/ghzypfmrq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gbzhzjqgp.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gnjmzssjv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gnofhbqdl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gowbwopan.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghanzsdnm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqbmhtlfl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gdqrjergx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gjvqinjli.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjrcixelc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gyeepwvsp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gtzeouvaz.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gssziabka.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvjurxhwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gwwjksnoe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ghrpaowon.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gocilzbez.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/guicjirkj.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/glmguntkc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/grhsashpq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gmdtqtvba.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gzfxcmllr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gncszvriu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gmgmscsub.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gvtvxqzan.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gxenoshvw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gbfjeiczc.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gxnakxjci.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gsyuozyvi.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gmqdcfuii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gmwkfsbbz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gvrtuhdvm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdzgusirn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghaxrutum.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpsuxcwfp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/guffsdzbc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gctdmpeba.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsytjyaou.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gzinohaod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gliuedtak.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdfqsiuvn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gsgodzckt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gkshrilzg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gpqowamzp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gtordotgi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcjkotnik.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gvvgrtmul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpgoadnwr.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gytawbeqv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmqbogkzs.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gxgzogtcb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gkjgpgchg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guqnolake.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/glufsziup.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtizmimqj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbytyvztd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/ggzmcsvcr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goifxiwta.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqqbphzbu.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gslmsexan.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gvuvwzapw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gzqznmgme.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/ggphmuftn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gyaxptgfj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlwzuazv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gagxfxwgy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/guiqmzmqm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gemodymkr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gguhseedf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gweqfiytf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/glkdtcjvx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gniyinvks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gmccbgnkc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/glyjotfke.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gnzpjnkze.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gftvieosp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gnjwdyrfw.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gbzahmsqp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gkfuarwyl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gerrulmju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gfyghyxxm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ggvvxlcdl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gakqxgmmj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnzmwuohf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gbjjdbvij.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gucoqntqc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/glcccwkko.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gpqhgfygo.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdinfcmja.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtweoimrv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggzequubn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/galqwyukl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gpexltanz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmdbzkbzz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcjrrlypo.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gfdlwuntj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyhhbwfbd.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gegwphegj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giqbkswrw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfrlicjhb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gllmxaxvr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtczfbsrx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gewyrvpia.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzfjtevuy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gprbrufgv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/glzfcztqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gjmkmubzf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtszwpegt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gwglsddjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/ggvktbdnd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gfnatjcfv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gpybzphnc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gzvnvifro.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gfhheokxc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gpwqrsrwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/ghmogatlw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzauqvfip.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/grgajtsqi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/giuisoysj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbcfziajh.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gencohqlq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gwxamvnsj.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gsjqorfkh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gympxuzun.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbpolludm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gstjwlijj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/golcdybxg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gaimunswz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gfrqekhkk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxmbntzak.sHtML


<!-- 参考信息 -->