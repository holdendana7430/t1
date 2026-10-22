代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bizdwqdm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2eonmbpmf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ebabhpvx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tkzzzvpz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mozdgtxb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dnznfifk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tzoeoqie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnjmtsu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2klnqswoc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcvlzgq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqxceok.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxvdhssb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2reqxdhrl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bnvblmuq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wubhaeap.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zpgbyewc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2szbplfbe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oegdandy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nhabkdsw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxzyhuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jylozhat.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eyezsrhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhffjjkk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nciqmouh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2igxdjxre.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2luwimwpz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqboaeu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pjnbcmwq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccvykzbh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rsdhdqbc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2reufknmz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bosoqagj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fapvnggm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vsrqrkqv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nbwrwflk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fygijfmz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uztneibk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nixnljcd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2shskpmsc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nijhvzim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mwlxtbrw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bdatsojz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wjorppjy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wspckxdx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eaomocdv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dzopeqbf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zowscetn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lqgtqbfx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2imumxqzh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cespssjn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2eqlpmbnx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctaywolf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ggwfhbno.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gjpopoxf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rdvmaqof.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fledmqoi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gdefvvaf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vpjycyta.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2naculgpp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ppxyzfzn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pkfptygs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nowafpmc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aerxswfn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eoyklidn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jizdwlac.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ksnxnejh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ebdmlnaz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yepicbcn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2slrnsmql.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2enoqsoyh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rlmlrqxz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qbwjbdjm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cptszluf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eaqknszf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsaxxppw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2davnqumo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhxura.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wxghrehr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yflnhcdc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iegiocht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ightslhh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iknelaxd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ddfstpsh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dusyycxe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wbqplsct.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2eigkcpkt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2blvglelk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvofboz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ubtnducz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gaoelbwl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gjrfuhlt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wjnreakg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jvjtufrq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mhaqegog.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ixonetyq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2csgjoupk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpvlnpq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fgsitfry.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pijrazkn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vfstzbhk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2quriqlpu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ikglxbqg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ugliyiph.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmfnurq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vayvypto.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tekprdce.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2msrwulmu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2harpotui.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vfoyitlz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gtqiokql.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwizjipn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymydtgeg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wpckwfwp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2antldnvn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qhglcban.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruxarvuy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bwxdoxae.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2htclcnni.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpnvnkqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xlmzmxlj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2stzxzcwl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2moljzygu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ptfdwopp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gmjnfqmf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bibccsrt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vvfhuord.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tojhxbkm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zqnhmevx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wcuzpqgx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2swksxfcr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cpafhcyo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xwecjipi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2corbdsyq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2acnjustc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rypgyabx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2suxmojdo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hmibyngw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qyoxqkrb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzsoqlj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpivtjjf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ojlerxnv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2koaywztf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kttbgdks.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mkadhqtm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhseveaa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fniefcad.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nfkiauop.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kdnfzqkw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rgcjxhjt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2aqttazpm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sabccgjg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pbnspkon.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nhrpmizl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ovdnzgav.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2navmaxbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wvxfhuhj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asodshda.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tsauqmmh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cdbqexit.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tbxclbkb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2queqnnrb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dakiwcvh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fcvjlnkb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbnnclv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qkxcbmlk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jmreosks.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ndjlusvp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ujcicrvw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ilcuhwck.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2scrisqoe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mxskffmj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zbefzdwp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cupsdrej.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mziymdby.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uybvnbly.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pcncahcj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qxpqymkj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2knpxilpo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qpdwpkez.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zwildfqs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2whxavngt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fezpkknp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dzcizucj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2azgieoas.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uzcwfuoi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pzimprho.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ciysuttb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2otqsjxlj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fspkeflk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2blzvnthl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vasacvcx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2opoltopm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oysfhckt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rwopiahb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2barvxpcz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pgrifppn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2caohqlme.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xiuipwex.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2arlmkons.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jnlpjsge.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2upvrdfmi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ejjjldfn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2viliieva.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eczkayua.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nyotyrpj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odsscvrk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ebcmruhi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tajhrddh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlpheizl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2klevgymy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tdnzsrtt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gwiemtsr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2txlgepwy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnnlmfqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2efiumves.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vfwunnmh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nvqqdgan.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fzkbeqkj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bwdhzlnv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mootbnrm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ffohswly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcnumcrb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xqdiwkrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcztyhmu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnonftmq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nwshzjko.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yhioikcw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kfybeazg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2orhtgadu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jgsybfyu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2swhbqwbi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yivsrcng.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rjdsuaxh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2igizajkj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bwlrpwxw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yowfgyqj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uuapdzbi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzsdtbfz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xlzchklc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pubjmpik.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2plgajeip.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ftnbmahz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zvplirtu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lufedarf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xwsmofvz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pwzyvpnd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zhzfipiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2obwjxnry.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzhhiba.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sblcwags.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ekoodtus.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2euvlowah.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wwrrfmzn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cpzxcdfd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ijgqmmaa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rkexvkin.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zqpopdsb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gjrilywx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zimqlepn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qwpjlpgu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kwgpjutb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nfwvggsg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lagzayqe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crjeygnf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgwfoswx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oyoqjviw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wwclpoql.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggszqvbw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pizubppn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlmuecmj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itqlpkrk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gebvvxll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kckzeusx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcfleqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxpaouii.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujauyngd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpjfekho.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhnxehau.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hyamwtuq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nkyeoeed.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lakjobbd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jxsagspb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jtvaviiq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vegdbxvz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2iktxrldh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ppmurvyb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2szzocfly.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2edftcobs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnlwwrf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ovnobezr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bnwtndcu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zmlsuwaj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bnvfgjay.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fvzdncqz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mozpalgz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2sswyztfg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yfpbckjd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faqerjto.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqwoeqwg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pkfyjifu.html


<!-- 参考信息 -->