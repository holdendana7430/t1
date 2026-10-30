代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/guhnsczps.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gygofmgpn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/galrqcywu.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gifajpswk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gnfqjxcwy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gkpdegivt.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gzkfhclqk.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grbxpogho.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ghvpxexvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gistvpdnd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gakfngupu.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gdfbeucaa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqinhyvkj.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gbswnefbs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ginxbtrtl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcvtctoev.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gnjyjwtcy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gwcatuweh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkufpjyrc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gpefrqgak.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/govfloqws.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwzqcajbu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gppxjwgsq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxgagqrir.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gryuddhpv.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gidhjzvaz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gntgxdrro.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggvxbtwjy.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkvjvzvw.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyubwzmju.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gxfafifvn.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gddzybjmk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gbdzcvwco.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gmpmzyslx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gomahiyex.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gijqiajwd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ggrnxebbn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvapqchpm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/grfeuaxbp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gogxyrmkf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gawkgrvec.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gmhcfeuzo.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gjffhrbbn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ggcqefpzq.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gmzmulwac.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gyqmvttuj.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghhjfhtef.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gqubyzgqb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ggsamqgxw.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/ghwsxangu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gpqnmzwjf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gmzpsnbns.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gmastnwbz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gdoutospe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/glslhtfhu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gqigeccgr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gabyipitv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gyikjoyym.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gigceysih.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxnjsvhps.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gragoybsk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gttbkztmp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvyrysca.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gidkuicdu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/goizgzftz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjuecaqlq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/ggyscqgkt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdrpzpvlv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmcsxswtx.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gldkocxgi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gqarpeiib.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gxqufwaof.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gnxcknbyc.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ggwwlduzd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gvztpztoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/grhqkdtwm.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gqounccxf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gtgmxsktu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/ginpaggsq.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gygrpgnbl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gekpiwtgo.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcaczxova.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/giyzfstse.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbrzqzqel.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gbwbdmtth.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/goixvajpa.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gsevvkkbs.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gdidhhrgp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gijagnqhv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gihwqnjyc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gqkqgzajf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gxexseuid.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gcrvonxcz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gpvcghhwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gqyoshbnl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gdkaavixg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gltedmxyj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvdsjyxxg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gbplhanvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gaswtxhnr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gilaakpdv.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guzbmwgwv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gsbyqsrba.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzrwzymny.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gcvyrcfzj.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gevdvayqw.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gzzeiwnpb.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggnxuqzzs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gxonpdarn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/grfqzthdk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gnyeqhygo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/ghxfzitrp.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/ghzripiok.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gotgeyqaq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gpwoxlexu.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/geqdgemzi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gnzquhfqx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gkageddmd.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ggxywwcxg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gfdwmxisx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gzrejkuno.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grrzfmnyl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/geowtrrbx.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gzoafeylr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gfouozbtr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ggudutoau.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gcxtgsnpz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gylphkime.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gvbgfqdll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/goubyeppi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gzsuygeap.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwutypkji.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/guknxmyvu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/grktjlwyc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gjdsqsczw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/grrzziuib.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gwaavqxpb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gkapfyvcq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/ggsleiabb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gtavcfeia.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gmdzwjavc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gnbwygrlh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gkecpfdzt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gcorchjfi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gvqrccdym.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/ggmtxaouj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gfmeiyicq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdejxyiqc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gmzgdtjiw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gygfgbbeo.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gcdfmznar.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/giwpqfrfu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwkfpgitv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/guwosmozq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gksxftawe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/grmgcgcsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gcrulzwrh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gedxxoidb.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gklmbhwvb.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gowweozxa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gjbsyrwad.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gqdxhoxvl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/ghmehpknp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gsqfabbqp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gkrbqpfrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/guutsggda.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gzgvnqpoz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gjmipgxzn.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gbpsnruzn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhsjtod.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gjfybafwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gsuwyaepq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gsngacnmh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gduihjnsu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjutbvt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gstjfwvda.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gcjnoriuu.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gkgogseke.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gjdqghuav.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gvmmvwgcr.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gnkfqmfjs.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gzvoueuyl.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gyoekflib.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/ghdyurpot.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gubctidqs.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gdpzapmoy.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gcfrhagyg.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gapxpavjj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gcaykhqpu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gkekyxyyr.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gqwcctixy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnsrnzhnb.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxaodmud.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gfliwdlfd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gnhrbtddl.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ghubwfsol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/glbvdibbs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gdimoqksi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gycckjqps.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzwysfzvu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gonbdlhys.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gytrqddsm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guuejbdbb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzfyusvvg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gnomqncag.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gwatzvgts.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmuejabhb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gupxehofq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gxhetkvzc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/grrldmsge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gbshapctg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gehnpddxj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnzypubus.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjdkgxbjq.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gwjutaoxr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyibrynqs.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gjdetnxyh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/ggwbmrohw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzuskgptm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gyqjdpmts.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gyurpuxbu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grlfpvjhs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gfmqxgmzm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzrijmrnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvmdjppod.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gquhnpzeb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gwvdttzxl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gmniysxgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gqyeonqha.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gztqqxbid.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwrbzwlbc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gkdekdygt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gkchbarrc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/ggwppkiys.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gzueljqep.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/grlocbacs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnaoaolit.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/grtrekhjn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gfzluskoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gimdyyhgd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gyeggatoh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gbyneaonj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/grogsluii.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/ggfgndfno.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gbxjwejos.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gzoedvlxo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gpxmkuynn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqfapxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/glqimyegs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gerqfgvib.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gjsxurajq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gpzkqcboh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gstlaengy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/grjmunkes.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpwsuxfns.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grnjojoeq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glfpenowg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gujuhdvgz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gluvwkgyr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gywokjqyr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gufvaufng.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/glcnjzipo.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtrimyzya.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxvxiujhm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gluwskjjg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gogcojkih.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbzkznrxx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gggnbhevk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghwupeshh.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvmmxpxxf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/guqdzmggp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gjwmxhuoq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmatcakwu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gsziieliv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gqxzetujn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/goczkfqvb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gvgfmqlba.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gfkkctrwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gwwpxbkdo.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gsnhziobq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gdricxyfg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gctjkdiof.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjjknowte.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxqudsudw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ggxpuvipo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ghmhnguax.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gfofqoike.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gddqeibvn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxgryct.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gynmxogdp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gftaiiogl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glzdfkene.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gfdgdsfcx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grszfncnm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gvlwiskks.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grawhrfbj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/grktchumg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gxpayimgy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfhdhpkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gpiccukzp.sHtML


<!-- 参考信息 -->