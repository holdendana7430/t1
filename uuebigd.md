代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gidgyjzwh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfsayurie.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gknwtzbnf.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwlgevawv.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gfuitvese.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gfkffzhgv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwdkybioq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gdlpjurmj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvixtqpwm.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gsrhdhxvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmkoeutiq.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtgtekvbk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gsttfprjw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gsvwhapgv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gvpqxopah.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghlvvgbee.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gjilmoard.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gwzjffbpy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gcidqgfaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjprgsvdg.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gykvrnfbt.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gbgpkkyvy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ggffzzrca.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/govzmakbd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ggkwnauam.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzsugkexf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gcfusyexz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gxxnmsels.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gcpaqcjta.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gdzabuaum.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gawpumedh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gpxhpgrkk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gdxmxnftu.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfomxjpts.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/geoggcvdt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gngjjwoem.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gvcmcbpjn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gxcwlpdet.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gpdpntuqw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gytmssswi.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gcqqgqkhm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gxbexxuay.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjbbfoxwh.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/goheyylgh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gshanrrol.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gmmunyoif.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/geppjojny.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gellzswur.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gmojybltv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gwohekbao.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gnmhtapxb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gkavknhyk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gndlulpep.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gxjnizkuc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gyxycevco.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gigcpecic.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gvontnkkt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/grgaroxdq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gdmecmrqm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdzewvaco.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfiehvnkz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glexqtfqt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/goyjxqgqc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwdwwgcky.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjfcwjxvk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gbmhkpqwn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gjkxudhcd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gehfpkscl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjannnrfr.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/galuyfwbj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ghxpmbkkj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gzzqjzuan.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gbidywqeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gwtadmpwl.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gvrxlngpb.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gjdxggfzi.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqenuads.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjqbuezic.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grntkixff.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gihcnbsvp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqfwqjpsp.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gpebglhcw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gtmugdrph.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gabebstps.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/grxbgzkui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gifcpciur.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/ggircscxx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gobuzksgs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gqakraedj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/giguaujyl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gqhpqnkvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/giowjnxdt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gaaswgill.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/ghieoakvx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gxxtgzwuq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwujxpksl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggnvuodfj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gluwuodil.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gauksfdtd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gbzpolowg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gyqbrtkrh.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gftkdewcs.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxfqjxtfw.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbhnolknf.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gnbhzitnq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gyhysefcg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/ggcijbyty.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gfebawzvk.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gapayrikw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gmknwfstn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gepnjgook.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gfocvzuoy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gvkuywlzh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/giwkfqlnj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gycjrmhxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gxtzizoce.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gqubhoxal.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gipaxjuvp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gygqdlmgs.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gkhbibdmp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gabkgbnbv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gprbqbpkw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxrslpons.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gxtcbsfau.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/glkvltydq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/grisvojvw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/guhhdtybj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gylrnkqlu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/grqlxxxbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gqufqnefh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gonbkeexv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gzgmqwgyb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/genttxxnt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gipkhmagy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gtteolsxd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gwjbrnjvh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gcwbeqmaa.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gremlvcwa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gdpquchzw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gngpzawsz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gcyvbuqti.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gvxfoghde.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gfxziwdev.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gfezmizur.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/goqjaygrv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gbsoxqrtk.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gyhjevsvb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gkksmjuuh.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gzypycndz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gejhiipsr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gbzqmjcal.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gsqhdrukx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gnwzzshzx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gqguncsmk.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gtwytjgat.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gglnrgspu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/ggywncpqm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gmsmnauiw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gtaxiazqm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gliktldqx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gsqfvdrog.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gvhdbtusm.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gykwftrwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gosxmxngf.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gnsbpvppc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gxkhtcjyp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmvfgqefn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggjzyoztu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gszjbtqhr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnjrpolwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfxnojn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gppivfauc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gncgodhhr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gromlfufm.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gvsbqfvnd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfhfbspwk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gmdpcgxxo.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gumqocjxy.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gxyctqglu.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gngkhiugg.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gftikvokh.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/giztnewlz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/ggqucdgwq.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gtxcyuhhq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/grpdjdjbd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gdqyrdinl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwrtsexhw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gcwnhholn.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gsvmwrvqs.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gyjckgkqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/guqbdtuzj.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gfbfiatfo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gwdpkkxsq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkjgbunrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gtuohqjcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwwogslcf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gnzjzqwbp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gxnsqgzuc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gtjononuh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvwlzqjgz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gtvnocror.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gnjsbjqer.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gpldqqyna.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gupphvdmf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gskuaffic.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gyjvooirb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnxlhju.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gpcrcokzk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gjqrltjuc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcppgxhvq.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gybjbezly.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfygultyz.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gwqljymap.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/glbrmkchi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjdataoet.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gkzzhfevq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdlwwrxbz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdydbadkg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gzjqcdeuy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdmtvnvvl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwszxnzbq.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gxqgrrzcq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gncvkolka.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gwhudmrlc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdmkfsudr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gsnlfdxbw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/getitafmz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/geljgaypz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gjplrnogf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/grcvvmdmo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/guwtuxwzz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxwythmbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gstlbunut.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gypxnonlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gglqsvytd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/garuzzpom.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gsxbmpoqy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gnchwfjow.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gwnjaxqpd.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gvptvfalr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/greadcwaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ghnxlzdjf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gvcxbkoeh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gmpgldbfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gwmfxtxog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdfldenvp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gluhbcskh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gvwnvafgh.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gorwtawpe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gruqpqcwk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjthxbjno.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gepmmlwod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gelapmhsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ggveuawrv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gqxscpufu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gujnrzibb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkivjjzsn.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gazrnyuxq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggqicuatt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvffdlvam.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gulfhdwyj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggsmqeocv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmnqavcpc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwkftfda.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfrgutiib.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwhiprzfr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/goawngmmk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gkkxieozp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gqbirgbeu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gbhtssnzu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gtiiwgjsi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/ggqgwsjoa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gltpjozju.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/glxavsqoi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gjqwqylrk.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gvpvkwdbc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gwunbxhsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gngyyosuh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpnrnteby.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gzhdskzwd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggmgjaeiw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gjmaowkht.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gngpxjupd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gpnjbgoid.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gpfqkuplr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghzgmhwxa.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gaecbyfni.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxsmzlvex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtesmuzen.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gasraiqay.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/goxwlirxm.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gruwjgauj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwsktubjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gwtfofimo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqqkeycxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpfzhkkmt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdwqrswcp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gozuczmmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gupwobvgm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtmdmfb.sHtML


<!-- 参考信息 -->