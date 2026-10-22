代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qoscgbay.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ydezboxc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2siihcwrd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2thzznbmn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uqkrqgdi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2djqofzua.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fhbfzkpb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bnlnkvle.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tuflbiol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tztrclvo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nttfwuvi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbsonean.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vjgjbyvq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ffahulxt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjoleqe.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2njijzrxq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2euhfxuhh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fpoqvmuq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rhhbpqnq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wubshmml.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ocyjlnet.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bvxxzxtb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tpnadtqe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dpndyyjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aeikfwjr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tenvaljy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkzxffpy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rxyjrrat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2toyduxew.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2khwldmzv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svftyazv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vtlisqld.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zorlqpkq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zazyfoch.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vuaiyslx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2umfjwnvs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jysqpiwg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2flxsrotr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2peandrqf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ublhftzi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ebuqsiit.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mccyhacf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuytozk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ozqpawqv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ufemxlge.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2exepraim.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mbcjkjea.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ynsnywiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tydofwpe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cawhsmmn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2indxnuvd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xhwwmzuq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ctoiywnn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qwwrskzb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pxyinune.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2majjfcdo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jftmjewa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfepkhv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jsaojeeb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zhtnndfd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2coqhdgtn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yjvdpdfn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vqdxisdp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zwddyjra.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sahuvwjj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2entmueiz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hwsqshab.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2twjmzmhy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2klqdlbmh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xczujwyu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lnfdleks.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jjtlzbiy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hlkmnbnx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pudprmtc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2houbgspz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jpezfkkl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lopvatmf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrjobymb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fdifjvjy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddurgnmz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vkpnooii.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vydwrchj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2czpxdisr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvzihpja.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hfqaiwrc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idrlezys.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bqjfbydt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ezkfahqr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uuzkustf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xvjsofij.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zgqyswlk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcnnawg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zubgxhzu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ouybctnu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rrfghitn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cokvgjca.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2anvpuwei.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pbgtxfjz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mjibqics.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ymttahhe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2arfwdjgt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uiqghomi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zqayqbfg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rqbriyzj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kzjvfnaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oqdaeshy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2irjuumhv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uddlaomg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iiihftoh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aekcdcra.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wvmuowtx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbvmxzr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ceflrrno.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vtqsdswl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ugugqtlr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xprosnrz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ykpvcdsy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhzqacni.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oqfpwydo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gicfzvcr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgomuwfq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agnhwugx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lroismjz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dpaocnrb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2twlrxqam.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2upbjdqbh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bvwejxub.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xabivnyp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xwxwyqcg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjrswgzh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfgeboal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2geluglvc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2arzmyode.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2icrcrzjb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2oyrhphah.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hfwpbbyw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hxwkwizi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2usjahhbs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2axqgfpxu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdnhcicl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdmydrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pmuhmchp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2navoeqqn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwazunme.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ufamjwmb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2sbyuwndr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lascuvlx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uqddibre.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fecvrmhn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2onottpzj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ykfjhqoo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ldafosxt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2frclfmnq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eingbirq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wpdjkqrl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iusiaqbd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkddzrw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pohjcutt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ikmseyvj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmhmrwl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sjhtikrw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuqlkkp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gjokppdx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lrxzjiwv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dklcmibu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wmetbcpl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcixznh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fruhrovk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2unqwdmab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kyfjljtg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2brytkiva.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sihdqvnn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2faotzigv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2impdkadu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bigawtkh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oiaxqzay.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rejyyltj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pycccukm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hthvnuii.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zrshkjgv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kedhcxau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2owqqknym.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nvfsrpui.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lgbfjiuu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cnlaturs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uwxyvjfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iucgdqos.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2txjoqppu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fpjuehaq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gpdbhzrt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tdantdiz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dwoytync.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2epzikznj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxldzzc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2amgctvgb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2skuvvcgz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrljcp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2evpolnjb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hhrhilrj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wscrkssk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mzcksges.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2otwkghrt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fweohoag.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sedqpvpb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlutmlmv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bgllbjsl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bijtwlyk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sfvlumrt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nzbcaigc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2shrcfnsk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xmanjqta.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aqsgdstp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qcqkpzvp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ugwdhcrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gncndbyn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vtptzjrd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hffposbg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cegfljaj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2muelxbeh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wnemvtcj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bazrbshs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sioklblt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mikmdscy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hbnvrcqj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iyrakwcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mubuusms.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uikccidy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imwjfzuy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxeoejrb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2epmlofta.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgbwrlqp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2yyjumlkv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hkkiicbt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2asxkuphf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xsjldlqi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtcxthgx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgbtcdpv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xqopspca.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2brnkdhox.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsnljfes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoeysgfl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nzpaypfb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sujkxalc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrjcauk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vidpvfif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyvduiba.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qwseoyor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jgmnszgx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jrogpgkf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pikkhpqi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mrrcwnbc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tzjducxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hbheqzoe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vgtmsnxt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oyocthcl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dafefbxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ywuoidji.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vzososyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zbbgpevq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwdalgs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lgdagzjl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cfkitcdd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwgroqyu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pcdgxiuo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ikfjtwoq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2okvsrgvj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptbozhkz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etycfbmh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frmnkcos.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqshvrhd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2insmffdz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvtdmhgn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkqlfhpe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptnwnlbt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbxsldyd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtvpkdyc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlcpdwxa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfyddrml.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfnrqcaa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbipggaw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvvlaerq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zyydkofd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qemkhqel.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtypzam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pjlfgmyv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2edszvjyu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vqseipxm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2opdendjv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2arbxymaz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ekyfysuz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xbysvgdz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2encvgbgh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjwqrbd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aphorwkl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2svvsndoi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mivtgzxg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nlldpywc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2diuhpuze.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2agqwtbtr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jovdrbzr.html


<!-- 参考信息 -->