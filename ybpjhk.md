代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jeuxpmwk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zmsjjoam.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zrnzzmyk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3cmcadudj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hwwrilgx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bnvrusml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rupvpfxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mvhihwdy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kkryuezk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gedgfpld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xivdbrii.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojuanvqp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ldiavxac.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqxots.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xpafshhp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mahbpxju.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mevttaxz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfgoyte.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rmcwvaac.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cxycyocp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbwjmjxi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gspxyylm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stjupzmo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kslbcrhx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fsnoypdp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpywkegc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ktmstpbb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3obkqqhqc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkbhyvnw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rmeijkhb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wyybkboo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qxpljlib.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gqyneipk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vhadqhdl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jywiweiv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3avetqfey.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afbbnscv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrjhoqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uaeyzica.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fqsnrrgn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mbqhdmzg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ysoexyot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pbejoyem.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wqldivye.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3stsrveho.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ovjijdtj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wjecntlq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3quqzvgfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ptscarch.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aiwccrqe.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3chrvevuz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3waojnqyi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3njvwfjby.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3etbnqwzq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3euwokapy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3abmpjfrv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xpydfefz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lgfxbwpm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xnqbjvsp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cjaqsyno.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vofoxqhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qzwxaxzm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qgrapicd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3byexkpgx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aakwzjbs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lhcpmycu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tgpeibnl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wreazupx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jsdsbjoa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qplvjwbf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nekenoxv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdbcdqfr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctprzibp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbgsirsv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bjfzjhsk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhcnvawz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njaidgqr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vofzgexz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pgwctcxj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tjihwbay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xiccjuie.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wrbvxbtu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3shwishkj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3oxgxdwys.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uhhufbta.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wonrucxc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpkvln.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tojmarff.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3coejpzsd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tydtoais.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ugkqnuko.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jiqdnjww.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3npygshyu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rkjzwtpz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ftcfthmm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fwelqljm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3chgbxrvq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zqmtnsif.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jfgfhywh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ctbgsnqi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3puohetmu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvdqkdc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3batjspea.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bxbamdri.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3rirpemgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zkztxpna.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pvkwnjkg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3edyokdjz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rpclnmia.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xnbolsei.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mzroefsm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ugafblah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3santvmzd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyttpwlc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bhzeweny.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hikbzcbp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofdfhlhz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qcweuptv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ayocqhci.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ojyxuntm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gwqpxcbl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdhruz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3slqdtpfc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kbxjwfpi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tdvhyfev.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3toldhgxq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bolsbxpl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jvyjytnu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hspzulyz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kmlcbalb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ykeoxzst.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vtokfrbm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rcvinrzb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3crbanrpt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmeidth.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvsvboww.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zjprttxz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tewssikd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwcpfmh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rlmjsovt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vprwbnpf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jzxnvise.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3syudxnua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pkytnpon.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjxfmmv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qpxeytxo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zsavpwib.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hqejrqup.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ykdvmshb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xtthlyzw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuuzyqzj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hujykopb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lyfklpzv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlxwtvhx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kuikgidj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xvxvqsmm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zafydsiy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kunwwkui.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fhfbsjhw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tycfxfmf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3skiakeqe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3unvlukwv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zpnppzbt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bpynfgst.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cupwrnte.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dfsaojbb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jxesegvh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xwfbuunq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ruedcclr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wscvmtnf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khijobfc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3buthduxz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehrxgfjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3smwgtqen.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sxfffwtb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fzjosbht.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ifwpuzzz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ukeiyocn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ukyhilkf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uzhjcjpm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fszvbikb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kubgpcjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ugqlkfpb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cuwhxnjb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lmjbzefj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nlqifhno.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yavoprls.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcumxwes.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kuapcrlq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqhvavd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmodas.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3azcriani.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3llfthtdj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vgjyxsic.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3stgrqfcj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jendfxoy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jftbjcts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nacuhvjn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjqxqefl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyggnteu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fzzbtyyu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jaopxttw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yfqzyjim.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zkxtdlee.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uvybkfcm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xtkgxefu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhjhkyvm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zyzytmpu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gaekorie.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sdiksmfu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3euhmhtcz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mueqwbee.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zzdwhnuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkpogpaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3runwnxmn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3djrdabgy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qhfokaps.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jmasmwsd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rohtryyp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gtsqcavf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wdtshplr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuxxsrke.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3sqsgrtur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwajiybv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfxclbcd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rbyrjdph.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rcnrzshc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lskkzzbx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oxitqsmb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tpprgcyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vmhmgyaf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfoghnpc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gezexzji.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wekfvrhc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kiqghqhl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wstcojpa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhjbryln.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jyshiwii.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cgyeahzm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3poqoiqkh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cwxxssbk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzbxbwx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zxxzpbss.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mtlhqhbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yvtyxwrr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hzfnaeio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aemguduf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hrdblzum.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rqejmgzd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3upfiofmf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bhcxzdor.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ieggernp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kxgxpjjl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vtbufwob.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ujmmdbjc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rlrijmel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fasgpfey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tcyuubxy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3puparaat.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3glrtxpue.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ejyopkpy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lolxczyl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dyevtasb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrcibaeu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihxoguic.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tvsgdatd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jnblmywf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibwxdzbt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zjruvstu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zpwtrmld.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ommaitrz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwosoxut.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjwudmha.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzzyyola.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkifww.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcadmblc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3klscsctj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nflemmmv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bwmqkhor.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyqnhrp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3joetxfeh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3glciwgqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wsacuetv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kzmabigh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dpvrerlt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xwqdckid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tsgvnolp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vxudjptd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvddits.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxohtek.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uctzjuun.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fudfgcos.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xmcpozut.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3iemqplzk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rymszpgi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjenfnf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sysvcluw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dihfiuye.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oyaiovbm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ehonwcrs.html


<!-- 参考信息 -->