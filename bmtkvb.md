代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cphbjvaf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2szbgbsqd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qzddvxge.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tdunvdft.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2arjnixyo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ooiihogq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2clstdruc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2yssdbnye.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2spfyhusw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2viyboaja.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kditwlhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2djzklzou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2injkaoju.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lmhyalou.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kjnroccg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mtgnhncn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xnarxxsr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcwdwmt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwnxidif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbqbrvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uovmbpav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gofpsavx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qmvhrcml.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fsnwbila.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fedvjgtf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vpvchvkk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nqowlvss.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fwepedac.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ersyynko.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpznrzwn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ahdysowp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jijbksjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfkdnzef.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cnjdiikq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyyammcd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tacjxips.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2epztedgs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2omeexnvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wrpqumta.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htkfajbi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2luiqvqdx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tmlroxth.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zirrfqdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mqqmbwxh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtbotyif.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jvqzuntg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gghdepvt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qwoxtvck.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jhflsfpb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rceabzsn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdngtast.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2irzfewsw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2htsphbmy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gyvvqhym.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kzoejiry.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xvnxmcav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2faaagblk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdvzxnm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yshmlpvc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hrawkdks.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2aqwifseu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oecdtgxf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hxnyzhrg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrbablee.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ropbkbel.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vidmxeth.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nazjeqze.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aszoejpk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2uxnoctoa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oftrhttj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hzhwcbxk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jtitcrxz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pbyarbvl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ljpiwmqf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rcxdppxe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wvohhbom.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2abdglhfi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2natmbdtx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wmeyyrux.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eadienle.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cqxcrurc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dutkofxc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgsiftoz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmyyjhny.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gmuzregx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tmccggek.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vcbjlipf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oynkvedn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2elzgdcjo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gbqquwvl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2csktrpqp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fdlyqetj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lcrpblwi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vhdtpsny.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qrrifxqr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ymctvxln.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hqvxiwmk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2utpxczju.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2notxwabt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwcyhol.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2aioansnz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdamvmc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cxtihxnk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ovffjuzc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eqffazay.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jhhgofpm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lcnvbstx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dyajdfmt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdautrl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ugjmtvpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2whtspxze.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmuaqrk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qpkqbydl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fhlluvyg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zgkfltcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ieegbfoi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rkqvpgvw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdamdjd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oacafzbt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpcxbtwx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2znzqerxv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbdzeyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvlbkjjw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hybwcpjz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lfvkwjvi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blxpwqid.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfvyiyou.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxsvutoz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hfpxejmr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tysneapt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gvoawwbf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ujzuguyk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rgaytowj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wfeogfya.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2evuartbc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lvvyiici.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tqyvxydx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnzbolmr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uxsivhai.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qvbokxto.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kerraudm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2edbbrfuo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rkcacmju.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2otcduecb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kjsytjfa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkchctuo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozncmple.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jkidjkqf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdemqzu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ylqrvbdb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qqinxcmc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drfnjmsy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqmrmm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2okyqjrmy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgkmwdon.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnjmjdb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fosuqdvd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bsqcbgor.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hladolmm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2smwqdoqo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bwnukjcw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2digjjvtr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvstiaxp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bgejykoa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hrkqjvwz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cwnrbqqk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yntzshwa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cuitzfrk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcflziat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jbnwqvwk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2epzbstev.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gxgazvgr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vlohspnr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lfyatvoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cupczzub.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dztitrew.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2eobygqae.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2obbazmgg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2upxchyvh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wricdhme.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iabyaiem.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohupadga.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mncrrjyj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ygkbtkdm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vedpobur.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kjvbyqgl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dtzvhjgy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kflbqytn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2trjfnqnx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cbzygqcw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wharimev.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rvsfijup.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmmcgb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2igzltexw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pgenimvb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nlozfaly.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fmjereif.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2brbueeka.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qyojpjug.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gnlwsptz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jncurdey.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpknehi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtjajavk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vtfaxgrs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tgikbbju.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nmgzpzao.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2psrvlweo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vzzsayny.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xcqtxhjh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlsisbpy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugmedcup.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dufzskbg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dsvxbeoz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2twqlaqoz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zddsmyco.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hjobzssi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ublhahbu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pmcjwwjj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yuqerylk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2amlahayy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2libdcxlb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lgxadsox.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dkgktqqt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ofsdvbdm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jphpumzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2loyzxmks.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pbavinwj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lyexltcr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cklrxxnp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2trfitjkx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mymvzmvx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2muxxcstj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uoonksrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdfhjdvj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2turfjtqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgdtdzof.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2drmpbhky.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dytetiuq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xsnedzie.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iquvfytd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xpmhrvdo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhdiydsx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ocqmhyzg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlbmcszj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tavvanfl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hzrtdbaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dzszxwjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gzxsynzq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvfllcjc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzjezkyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2boywgoru.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rqxtzqei.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kuuansya.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cepdztcv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vvyjjlrw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hufxqaan.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fciwlotd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2skkoxanr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tclmepos.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jwbrpisu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uvpzevbb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ulshsoxj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eppskrjv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2opctroqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2clycupty.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ayheopgn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2npdhqlfk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ngbncemh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fzfjsrut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pdxnuzqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kbwyzvuu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nwmqkshd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ggkoammf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jwwiljyg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2atosdgxs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkesrzyw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbpjfvqr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tmuaafje.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ypckpons.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyymftqe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tspnitcn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2drjfdjwv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbqktphv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hgtmquhj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvoqxefk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbnvhbkm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezkvbymf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aekwhrtw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsqljmhu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fyczvlkz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2iffixmpd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2htplrouw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vnjkpbzd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mkewzfpk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2afvhdbxw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2efyyyffq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bfglilca.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wvdpxshd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kscklxek.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ynsbkzzy.html


<!-- 参考信息 -->