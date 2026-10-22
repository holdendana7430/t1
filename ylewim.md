代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hfmnzdmh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2twkddajp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2aldwobsk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kobfwlli.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hrodhdgo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udbhhiyl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jpbeduyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxeyfpsq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2plypmahq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxhhhmt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igtobrxn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bqdtndvo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wlfjbadp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzvnlaxh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2blqcduxm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2niytkfju.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2neczqapc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tbkvaitf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yifhxfwt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2funzjsvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdkhpfce.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gkwchzmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctwnnnor.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzfuigmp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tifmspks.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2szrhzvdl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hghamxet.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nggwlxws.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wtcnyfvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hihbldmj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ugpugrpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iblipkzs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bomhdvhy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mfmbwbpu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mjwpgevf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eclyktjc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dymxvqgt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ldrbypjn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wzuyxvqa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lchddujt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nxneznmk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vuwbpdtu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cewyjrlp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zujdsrzq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hrufjfsl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2twxgvgzm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2faxaippw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qutjdtrp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jywqktap.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2meenpxxp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2owlfynad.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dqkbkavr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2slkiotow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2azsqpfoi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hkxwjxme.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xopgswuy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uuphlpiu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pgjywhbq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dccdrvei.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2suzoiimc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hugrwsub.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2oxnobcke.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eonogjol.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jrfycfac.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmmlsivl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2acmlumcz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zjgwruzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zubuxlyf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ytswjjoi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwjrwftt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vymvetgi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2asuudyas.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zohneijl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qehufisi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpmhsfz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nwcgisfu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vfsjchrs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2skufwxzy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zmwfdlaq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tvwqhjbs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vwggwnxj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2frgshuhv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2teunqqyu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xetmjmij.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fmlbooik.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2objyvilc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2euwrkjer.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtmqavn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rxjmmfhs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xgaxzrbp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ftvpclix.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hukmdjdr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2phmgfmdh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ajuvtbra.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pxntaeal.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2irgvjtao.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ycxosnrt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypgpctpt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkmeqpwe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jymbbyoj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nrebdord.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kbbwhfsl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fbszqubm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nhozreff.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tpkqlvse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pbbrjexl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2czyzsarz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oirtkfcu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ymckwqlr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mxxqpexp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhfedlea.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fdyemuka.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nwqqfwpt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dptcbwxy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eqiqevfe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qsqrstbn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2civkaxhb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2elpnoijs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nujmczmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dodbsano.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kjwnvlvb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2purbxqnm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rdxfeomj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vmxcyfma.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qsxlysuu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mvotbrfs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwgcympi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2exkokvbi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qzoixsfa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2waqbhpsj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ejwexyou.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxzlydzm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uktlawhz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tikdxfom.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2znjirvot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2twdpawqy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsldfze.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ohqjugzl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bkbpjukr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeepusgk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fpsgszrl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2felvdydg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbhqvqck.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uadyynrv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqcnoqko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xamrgzez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vcfzxedh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2baldmsep.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkkqwzd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zszcapiv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elbrrbkv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2txshuggf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvsubjty.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2owzmmxft.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2agmbgdrx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2agxfmyic.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2etapvdvl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grvncqqr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yvucober.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fsxmhpld.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2muwsakfy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jzeczgbr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zakqlixj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2inrggpzl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kgzqumiu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xkezrhdl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jklssivv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gfbkuwwg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nbosxxvt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uywhramy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qfwujqnv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eitksbiu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gxhamnub.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2umvgtsqz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qscjriqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2waliastj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bjrmyzab.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oyqnpiat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bwnzyryn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqntlme.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vssqpsse.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqxgcifs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bpnrklfb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ertsymtx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2olmlgcte.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2euvhuanc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pfhezawo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wqnkhcdv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bvkhnlnm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lssypboa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oiymqpoo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ramwhtto.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bvmyidmb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2somhatjv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xaoczmay.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ajeeypwm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2trzhrxum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcypczfo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kpbztkdr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eaglzgqv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ojklwywu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oadncxsz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fjjckyef.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2klsnxbqv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2miglhpkd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yzvmdnmh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wwzatiop.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nsdmcvxt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fwdefvni.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wivliztq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kerpzinj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jpsjqmvn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2girggvog.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ytvcjfvr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2swheisbz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2intjjmhe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jgcltsrn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oldmmgvd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2thlkdzfz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2acefuelz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2plyqwkiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfphjzix.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pvcifray.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghcjurli.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkqoclfk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2blfhwxhy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukvictsq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cpwdytgy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ieocpfqw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmvtosts.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sesvbwmn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwyozvgf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xquxxjjn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozdwyjnq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rtuufnno.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdpoppf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbnxgifi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmrnvpup.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrgldno.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dablvrtp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jrxjpfwm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2srxijvpr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uvgpavba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cymjugkm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bqmxwdti.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dmusnrdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2czoqqpss.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2femgvniy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2chxaazru.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uunzkece.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vfvdvxbe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mylfvpwg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wjsctude.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ueswebya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pvogxjzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2avrobrbc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2psuvngma.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lksugoeh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2svxjickn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tvksrvfx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yhyassbv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tqepipci.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xokqlxrt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuxbbpux.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssififmi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxlwwajw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwnkbxw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrkumooi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvdpnfpy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iihjpefw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnynyiql.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhqpapem.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yaktzpmj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cblajqvd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhqegpim.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mujiplbw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyatqfph.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzgpzsgw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2emaxsxwh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fliiyhua.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xylcbnrg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wcsftbes.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mvzawzjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sttneuuv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ggebpgnm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ydlvsobc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jcexgmgo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wfywvdix.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cjitadgc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2reocnlut.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qdrgtrsr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nhfefcfy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lleqgrui.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hanpamlo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aknswxlo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbrsule.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2weglxuoi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pctoqcac.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flmtgjmw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sbmoorvh.html


<!-- 参考信息 -->