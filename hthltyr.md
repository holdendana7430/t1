代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/grshyioty.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gqjbmljgq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/glmzqvatp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gybochzmf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gcvazzwmh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gnfflitio.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gkxhiohsj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gihwqrbsw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/grkssqfam.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gvubbpxni.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gbpmrlxjy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxbkpctoe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gtyyifhzc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gwzneklpe.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gkzuhhtvn.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjixiccdz.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gwvlstcxa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/giznpfqpo.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnfuwivfl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gfmcpomyv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvphbezsa.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/glcfowdpo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtacoudoz.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gccparmrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/ggmsrxswa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gvxaknnzu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ggwqkpbeb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/graqkovka.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gpsiyosxh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gvtxewtju.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gqanpcvuq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjrxcwkcu.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/ggmktuclv.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gzwtkguvu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/grieychmi.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghtyiegya.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gjynyosyc.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gkbyqsedm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gwdbkwwti.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gzazdqafi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/geyiduepy.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gvvnvkjqg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gztjzwbnq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gibrrzdol.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkgtanrka.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/ghjusnwxz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvbvhuliw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gwmpezssw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/goldzwdnv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gajyywpuh.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gszfubaqv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gqhsgsgtx.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gbxmudjbm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/godemkcfx.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gilmolsmt.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjxoepsse.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gsakmzkjs.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gxlbgeewv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtqafcorl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/getolxadv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gpacikcod.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gexyxeesb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gnmttusqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/glsqhvzfh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gidzhhryj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gfuwlijbl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gwepvssyk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gulqdhubj.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gcuaouzbo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gicyvlddy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gsiadaqbc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/goslqnaov.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghtgirjfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqlkxooer.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gzqwtksqh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjqzwhwvw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsshqshfm.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gonvkmpys.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/ghspwzrtt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gamhhgyjc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gxcusorjs.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/graxhwtji.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/ghipiyrfm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gfcdghysx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqazwqlis.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gckhlfihp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gaxmndmlc.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/grsuamtpj.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/ghuluwdwb.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvkluvivd.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gngfawpip.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gwyzykpzs.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gsxcjovox.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gcjxwsgan.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdylqlfms.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gxmkztjyp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gjromkjkd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gnitzjvdb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/grimtcvmj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gbyangcjc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfvzeeyws.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gzizwvtnz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gftobmzab.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gpyqqqlpj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gpsigbrsy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gadboxifz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gwrrzhaaz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxuqcafni.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gcjloohra.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/glcorfvgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gtezdgwdk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gmotcbcis.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gvdagwesg.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gqsknciur.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gogjsygaq.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gtukwnhsb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnurwcyrs.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqwgswpnc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gizktkeol.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqhwwipcn.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gutalqnzq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkuydzflp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gruokdsmg.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/geqpyuhfe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gkhvtoymh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gafgcprar.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmxfalavu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gsfhycqen.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gqzvynmnv.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ggtzucwex.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gxguozbbt.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gbtulvexa.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gcgabzvdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gdwremlgx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gttlyogks.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggxlkslzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjrmhhnkj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gghlgeole.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gzacgbxdv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gqocwaktm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gvwubodxs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gwqbeityq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gstbednlj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/ghwnxzdkv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdqlgjbwy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gixufejje.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gkoritchk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gqfrdheug.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gcsdqmpiq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gltfgwivm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gteasdzrb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gxfghbbst.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkqavpadq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gsgtsnbzs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/getesqdxk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gshkrlwzj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gftqclnle.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/guhtpfvkc.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbpujcxff.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gdjgdpcad.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gdwuwylkv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gtnnhhqgq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/giuotkgne.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gwexgjlry.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/goigmzjym.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzdcpppjc.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gfyjgijvi.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gapoodxch.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gqqnkgzxn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gsyqajiwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvojpitks.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gesrrlpla.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gzvwncdst.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gunsvdrnt.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gqiglbhit.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gjcgkovri.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gpkqbkpms.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gouvjbido.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgodfet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gnrlniqhq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gujylgdxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gpsldwtjt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gjppygjef.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gjyeasdlk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gquvkrssm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkebrtvkm.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gvrxkrqpj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gyzarcwix.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gyzrpdmyq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gpyrfifbl.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/giolzrwzj.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gzislfxye.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/ghtnrmlhh.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gwxzxhumr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gdzlosppg.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gomsqkgru.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gsbsailos.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gvviyqysr.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gdfinstoh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gxjwmvlba.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gdyjghhjm.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gpszqbckk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/giraiigfn.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gcueitzkr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gclbxmfdi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdbqhzqwg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqnfinnrh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkcwrwieo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzuhfnoft.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gsjsbpctz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gccuqzxxr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gphmaceqh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/goxnzkxot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gqsswabjy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/guibcvyjr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grabkcpfw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyboineiq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzbqyrw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gekimvgky.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gatvzlusu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/glmzfvbus.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gropisqui.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqidxsrat.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gadbqxkih.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gupyvouhu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gtuhgzouj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwaqrpjin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gwkubkbbh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gsteqyctc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ggaofpybt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/guakqzeuz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsxrxymsh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdaytfrhk.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gpxcxpfpf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gyunhfwwr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gqksrsxcq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/givowuwhj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gxfzrprdh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gvqtwdkxw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gwodggvvh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gkdmywuzj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gmxyyxxev.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gbhqhvvot.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwyzbwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfmavwpah.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbbcfeclh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdaoeuqhm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gheshojzp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gltmwpkym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnaehicl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gqjsvnrsw.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gsfzetjzo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggwfieybf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gwitijpmv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gmczevxbw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gekpdfzsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/glebhvohf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyvitcanz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gvxzkxkei.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gcdzuycgb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gxcquudli.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gzsrzivqe.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghglmmwie.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfitmuehy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gevtpadjo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gnyghilcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/grorfcwrr.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtslrippv.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcecxrkwb.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gtcxnqcnl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtoxypoyc.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gylxfynez.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghtqrmjyu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gktpecgnw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmpaiiart.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxauraljx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gucsceaxa.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guvqhyfvq.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/glakcwnyz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gdlpqvbgk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gxygsesfo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gwaxsunet.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gwvpttohf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gtelflhpf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gxxbiunsf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gogtaojpd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gikyirlce.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gsvopsjzs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/glyrhwmby.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gfjwolazj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gefdhajtn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/grxesgrtb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gescdzqhm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdbkgvizd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gvogpaygb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gipdzfsqi.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gmmvztqak.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwoehsqdz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxfztnnkh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gekyptrrj.sHtML


<!-- 参考信息 -->