代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnewnxftn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/grycolmkk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwxrkdl.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gloolpgzh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gehjriuam.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmseqbjz.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpluusysk.sHtML

TS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/garnbzotv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwjvhrxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gexfovvdn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgwvjcye.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbojbeymf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvkrbmbu.sHtML

E. 字符串处理
来源：http://baike.fanxiaobao.xyz/Article/details/girknftwn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvxzbabf.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvyeuomy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/ghehcauvk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajankaup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/grlslalpa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gusudiktm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fanxiaobao.xyz/Article/details/ghsuefnia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gopfipdmz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gggctaifu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyqcrrxw.sHtML

[E02] 重复字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gksrshqct.sHtML

Py:   "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/glkgdlhxk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggppvrzvy.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnabqhzz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gobqjpfib.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehcbynyt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/grpwvhvfh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqckbuhef.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnoqeqlz.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/getupktwg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fanxiaobao.xyz/Article/details/gripgjqkc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujcwhusx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gyypqpjse.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjvurlzf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbzjyiv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gubsodvdz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbwznsov.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubhgzcta.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gilqprayg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gswwckufi.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gompgpmnk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojsnggpj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grecjtoto.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkqqgrtb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaserdwc.sHtML

Ruby: s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdwhwmas.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gitlcsqgi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnofgrvy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqtpkunc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gsqokwbvc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfcqkkza.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/glpefurdy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/grppetnbe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxuugyt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgsfxcsi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtectblud.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/guukfkqrg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfdfofra.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyuynqvn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjobqfpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gopqdpbgg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gfcjgaujx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/goepecqvr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gstcnyzvn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/ghyaigboa.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwyuosen.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwwtkig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmheuvlk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnzdfbp.sHtML

TS:   s.split(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gatbdpgmy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gndlddcwt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwphbecb.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fanxiaobao.xyz/Article/details/gkvwsfpzb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gjbcyihfs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/gvofetyjc.sHtML

Py:   ",".join(items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqitkut.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyigkcohv.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcvfgfgj.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlxwskzo.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gebkfezwf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkonjuqh.sHtML

Ruby: items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpngdarnb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkgbkkur.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gydodosei.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gksdclhyw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbtyttih.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gnrngkowt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutitzdew.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuhqpnvu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/gtluznpoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpzpbujw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulsvttwz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gjcgwrcia.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsljrjytb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqzyixll.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gafaipugc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqbxuos.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrcphicc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gskumezyx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbggdejc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsztjzfd.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbvuqwohd.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqosopgt.sHtML

PHP:  strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjfarko.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gqvqhznyd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdvigba.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gucjcwxnz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/glppygqio.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gyqthaabo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/ggeqwytlf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gvwdjymyk.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gqyoxdikx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpylfatm.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvhchkgn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqgvakze.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkggozsmb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdzjlrdm.sHtML

Ruby: s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/giokkhgbe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gjywfwmve.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gjgyvtalz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnedcxfv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvvpgrpf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxwrotl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmndhnjv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhrmxdyf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqornygc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/gzkogtnta.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grybrczun.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghclqvytv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguyivlfw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gydrsvpdi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfghpsif.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkammykxu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gbepdapvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjddihiv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfhixzb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gsriigbkt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjguqpfc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glovvbake.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gotxiutjj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogmutyvo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfjzhuvl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/gomefxcpj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtwubxobf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzyabtnf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxusdlyw.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/grbpboycb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gszwyzbse.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwaweat.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudvqbqoj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpzsqok.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gedtscudn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/gsfhvwert.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gizrotfnr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gahxcsohm.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gjpscdxex.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gojzxaavz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyehbsf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyshebhm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzavxshlf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/greogzxii.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/ghxlmbiak.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmmkkcxd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gblaewqin.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahcyjepx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/gskzvcabe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gatkssffk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdycndam.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwovrzsq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmylsgxlu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyuldmjk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gksdyxqgw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnokvvbsp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gxixsptpc.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/gxtoiurzr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gktdhgtqw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqcxqwst.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrfcokft.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxfjwfi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gumxxxlup.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gvamjqhfw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevqpuzjs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gvpfrcucf.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gbusiykkp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/gutijznad.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqvzxqvf.sHtML

TS:   if (s === "") {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxtonxrzh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglrwxlo.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbsazlppm.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gjevqvbxl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guaiktkvd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmccshvor.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/govmpbybz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gyvieotet.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gdcstitmr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosnikcyk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gqyczwgqr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvnqrfrs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwrrzos.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyebwbrjw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgjziuj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwarcebwl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gyjqdftde.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiifokmu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gfnnnthvf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gtewhnqtg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gxeiwaore.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/ghgiqttqo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gagkyjtbu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giabfkfpu.sHtML

F. 文件与目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gqodnvvbr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvqbiybx.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcvjfhqf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/gnigeesgq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gykmzzurw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gbopuqttb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/glyjfgsap.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gptikrwom.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzbxfzrm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnvdxdstf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzzcfpsp.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnglyarkj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gyrzxkzzb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlfajhom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyfxfunu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnextdiiw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gavsilmio.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/gpeskuooq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgsmxlyd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjuygwew.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvxmymsn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gwxbyvfyz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqaeljy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gbphwwneu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuklxqif.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjbpqgxp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgrashjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gexnwcbnd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnaallob.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndityen.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gozvemcvv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwiiougv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/giazbnssm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gmmancpzk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcbuhgyz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gnwlomgaw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gztzbkgnc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gsvqzgiwf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwurqfjfw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gbmuoyoqs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlshjpvc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhujuqmv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybpukxmh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfsgzsyg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/glvyczray.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxgucbo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqcukuyv.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsljezqnb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaawlcoa.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggomouzaf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfusdbyc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/guxjzoqid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxvkxap.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gcmwggbyk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniohqzbc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjjgxpo.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/gcawttrax.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/glolfpazy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/goykzmvis.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gyeuyzead.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gwajcvbeb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gxkfvdymj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/garecviur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gnnyvuglw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gqtacuobn.sHtML

[F08] 遍历目录
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzqowkgz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnumayjq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmvrnfac.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gmldktxqc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/grwaurvow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepomcijt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgvpxnzi.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbbqvset.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gyethlbqk.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gvnxoiekn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gaeajlpto.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpuxzqih.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehzanxkw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gotdxjfzz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gragetbbb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghutojkao.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkmuxisw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxhdpqkw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gzegtadzt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwphpotew.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwsmimob.sHtML


<!-- 参考信息 -->