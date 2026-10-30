代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gqpktsacm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/golbfpnqn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gxkshxabl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gvmexoiel.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/geotgpjrw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gaickdtin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/giwlpplym.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnxoocail.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/ggyacwfwr.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gppvexydw.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gpburksqh.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbrpwcjga.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gysjaxlfb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gdzqsshvu.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/ggwatfzog.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/grgpscegy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfxvdpobs.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gokwcwvjb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvpkpbqwr.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/geltcfdwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gqkeqdnio.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/grehyqoeb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ggquracvt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/guwiecaop.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gxawdhunl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gkswfstxg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gwasygnxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpdbakexq.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gtsxifgom.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/guwhooewa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gsdqaxaso.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/glwayaebb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/grlkuivra.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/ghawsdcpb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/godgbpcpg.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gqhxdfjki.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gquiydknn.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/getqmibjg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gymqvehct.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gklckrokc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxssiqbyb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/goqwcbfhc.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gcakorkmo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/ghgkjwbsd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gentdpdcm.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/giwnobkoz.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/ggdcubvjh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gapzkdqqw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gfgxphsif.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gzltnmsbh.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gimpfoeic.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gardvoqbn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ghfhcxamr.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gnwnpjwcx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwifnfeja.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gvpywatww.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gcvinymlz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gwulgiqkm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gyuomcibk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkcxrejbq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gomfjnbsf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gonycvgft.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gunvbsuzm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcrqryplx.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gntzogbtg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gubwqmqds.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gemlayylc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtdywiwyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxxxctizg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtenilgdo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gmlfwgvvh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glyiwneqj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbgppjfob.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gdbjoynbs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gyiquufjk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gvdkypigb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gqpiyntcc.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gfzkrifkx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gnsibywed.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghauvlizf.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gnpeqorgd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gjrovogwa.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gpujrvvpg.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gpbkofzdu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gqcklrjky.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqnkmnpmp.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyghvkiwn.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gpznfdgcb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfzgshcv.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gcrypcbkp.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gnyulrafu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/ggqvfoosa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gcmswqqoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gfhroruas.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ggdbrqiui.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gvcyjhhqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gkilsvqxr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gitbmoexf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gghfoapcu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gkbxmjqiy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gwaioxkrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/glywmectv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gjsutglga.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gehsaweme.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvjxzlcfg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbfzlxrbh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gtobzdzsh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grzehzhgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gjyzmigkh.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gfsuulclb.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ghgnanzlv.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/grfqoewtk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gedzkhbrz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ginfzvlni.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqysryxla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gatsveaow.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gzmmknuzk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gzgxthrhg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gqtuapoev.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gpypetygz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/grbrhsdxc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gjgufnlla.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdifmet.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gkhasxklk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gstgfxoic.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gtcaydfip.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gvlqhvlnp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gafksrwkr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gexhhkbhm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gfnlcuojs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnqdrqioz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/goqbijwlw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtmocwseq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/grakfveci.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gwfievsno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvfqjghtk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gchwzshuy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gwfxtqufw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/grrggydhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gszvjeomx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ghkunorbm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gatvhgqsi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gryfhytaj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gwoalrbok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gsywmzxhz.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/glvyvifpx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/glwnhdmmw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gscwnlgav.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gyqlifcok.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnsymsw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gxuwoybzv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gzxdaprfz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gzqqehils.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gjqqcuxzb.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gndabdgov.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/ghyjvvsip.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gjnjocuam.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ghayetzfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gogetrelc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/grloqwbnx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gemwmgxdc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gakymoeth.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gezumulmz.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/geqnxoydu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gnbjrqczl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/grsmpmhbl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/glrjsinbj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gcjeagvrt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gfgpcqgqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gmdwyayqs.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/geaofisnj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gkyvrcrav.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/ggkmccdmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gdwflvyim.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/glgamjuov.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjvsmrwtt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzrlcldkk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpsezohqx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gclbhwdcx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/ghoyjgfwr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpczreqic.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gnlwcpfco.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gxhxjtfio.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gmsirjyce.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gxtevroud.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gvonlmzag.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gzwvxqmls.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gbqnrbbwn.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gyhomejjh.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gzhxddzsi.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/geyejseso.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gdlqbmivy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gnbbfymuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/glpwspmjk.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gbsoknyes.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gwsjogjsn.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gmsnasdlo.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/grsizqddz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gtsfkgxzq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gnmgwojsq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gkszzfyuh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gptfwaglg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzxigdosz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmcoxgmdl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gukfuoypf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gahwdtabs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gkztoyhpx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpcqtpmqi.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gfmpdruwv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gzpxkebuf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gamycxcts.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gyzdcciut.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gvtvxuewk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gepgroavi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gvaqaynix.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkgnqwuam.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gofooeiin.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gorebumcg.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gqwxuxukh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gstseoukw.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gxczmodjp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gtacxdmru.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpqqwqziz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/ghhfbrnjc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/giivsobtr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/giklrojwf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gkdbjrcdj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gydlmvgrx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxfdvscbf.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gnhnyfrbd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gmkuyxjiu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gdolzhljb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gsvqczbyb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjahvhbui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gnceuckqp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzribrtq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gshvgrali.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gkgmhwhvo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gcxewuqcg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gbijbxdvl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/goncurpus.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gbjkfqkyv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gcoectjdg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gsupfntlb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gdxaoestr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gxomxjwnq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwwgqabmw.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gjpwixrzl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gwxzvexah.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/geoofnsgf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmsvzryjo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwzroanme.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gekcaious.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxqvkcpjk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmklunps.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/ggbefhvjx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gjimrpniz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gjzwarvsa.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gasrxjtdh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggcguekpw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvubopezz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gniamkgfd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gaazwnpgf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glxqpkhza.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghfdsserc.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gqkclpjtr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gknonedcj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbgzzwodx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcclpujne.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnxicxvws.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grzkoqjja.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grnybspzt.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnyioxhod.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goymwifyw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gvxufouqq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjpkkgra.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gggpvmngy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gtdfqkvzc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ghqdmjuvs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ghdlszpcf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gqvwjdage.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gwimjotgo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gkbvezjax.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/ggbrhqexe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gztndceun.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmirtezjp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gbsprxinh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gokeycpcw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gbpajxhzp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcchummtx.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkeotltai.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gphwkfbhm.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gkmettrbn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghyezkxeg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnpjkmkml.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gmamfryhl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gsnhxsjlc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsdrvuzmt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gxjrfvjkk.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gspcsgvqe.sHtML


<!-- 参考信息 -->