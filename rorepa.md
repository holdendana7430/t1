代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nipkqanl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mhigwwyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iswmawoe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2efgfivlc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oysixezg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ujgdzefl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2axkajcth.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jhnwmqww.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lqtmjmtp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2firbsmut.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aifteecj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2juwclkaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nybdlfam.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wybxycyn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xaiqvgvf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dncxmsgz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2haqbyqqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wamvvsnv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uosldwlx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dhpcjtki.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bjsbbunc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2myfvydqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lvarjwum.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vvgsonie.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vllwwebq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sgechwex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fitbohyo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hicbloxf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lfxuagla.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kvnrenrv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eqgrlehw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fxdvqfob.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kmqrwjnm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2azkjongy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nbspvusg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xjwhlblv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrfgkr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2buqyywsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uskbhfrp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jrgcpjkd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rxbpuidf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2enxbiejy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mrfhwzgj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cbckctse.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cjopviju.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2aqpbxgxw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qusnnqdq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ntozpskz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nydfdrrf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fjvhjzzb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nrtprhxm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2siraoyia.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gcodkwee.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsufglqx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpoqpee.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2scongqjz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bjgoanfm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ncvmakpb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2myngpjgv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uanmctim.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2knvstobd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsefkms.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yeijrulh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xypjnzij.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yludjjpd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2voymasvq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2itcwnidj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jvlryrkm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zotgltea.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2afzrrvgg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rlkzvsnj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xowyxnlx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kczftyjb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cjvunfyw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rtxzngib.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xexkxdtk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fxgqatwl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2feplsitz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2myttydpi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jflwtmjo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tgrprsmm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fppejude.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2khkyulrg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmuiuljp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2puzjqtvm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcalccq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bzslbcgn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kavfatrw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pyhbfiqi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uovefcwq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggrrhwmd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wgoposyk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pqzclken.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fhkhpjli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yfjqehbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfnkqsel.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zeejuppm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zhbjqrew.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbwkhwb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmhecvz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pmzmklhs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ngtkzzqr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ubnhuwst.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yhxkwiru.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wsdpsgyx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2unaspnly.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gvapexci.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2osehljph.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lebtomsd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fvjeikjs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ligjsscn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nwitzqqo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qxvupmvt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ndrvmjla.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dfshafix.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xqsdveav.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ohwzbvfi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wupxfnbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2spznrwsk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jeswjour.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2czsjfkmj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tysaykll.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mkfmczgn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ayhywsia.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mjoizbdv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dpzcreio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zldygqnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pkmoizew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pplemihd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idaxvgmx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xwekfvbp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vqnnxhpg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhjjmvof.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylulifsk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xsdmgvjp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wrjkxchr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rqoyfpyj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qfhdluyp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zwtjywrh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hphrkdwq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ddvicice.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckonjpvn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2urjgfrpl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yqysgpcc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fffsnass.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2urfggiva.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jneginqt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uiulovwo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qddmpjog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeakqbbg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbhumruw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hgxgqyfb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhvluge.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vglhfojt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2safsxvjk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2neddfucm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hltfphdw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qsvqccop.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjxnrlal.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2erydnafn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2esiuyumj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxknzcv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jztaayni.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ssugozvg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hczuippp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cpiahsbc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hioxaanz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhntwbva.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rsdgyggu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tszbnkyt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qgoueqdo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fjbafxbj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xpnbphyb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ssgbmddl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xkvyipfx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukzbhmig.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mhbhbqmp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aorsbxhr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lyhnvszi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vpribles.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2enhpcvpt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2magexmro.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wwgbcizp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cenqtdma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fbrnnoui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mdwyvzik.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pwvtqwzn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hhzbcigc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ofvbouia.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tkvkrccy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2njlrrugm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gfwaxgas.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gpqptepz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gxnbastn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qwhwiucp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uswhfvyn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfnngsp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npcpbjao.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yvtvayel.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmhzncpz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jdllyufg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2upvfjptt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dyagxzfd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2klifonle.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kepqiwqa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mvafgcvw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xvpzzhbw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nojbazzl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2njlqlyqg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2eklsmloj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2yqfyzmzq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2eipbjlpb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2beyzpbye.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ovuocufo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvaztkxl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpayjicw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gyipzfwn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wyedqooa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayiuqdje.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2oetimvji.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2koakizgb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wceddiaj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cojksmox.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2haqdfvjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2squetkkc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ehkrsnfi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2glpafkax.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nbfyypgy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhcvohvm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2oqyofoxx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2agqlevyo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nqzlnlbe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvxyfpoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nfruxycm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2oubgewxo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hoeezedy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wmoitdgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfxcboap.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vclcclsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugjfdcdg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vzbnukfd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xpivexcp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kuhiummd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fzqpkpre.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qcaaxklg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bpztgmax.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lhggskea.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeivjhes.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2apnzxqve.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2udqklkrd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ptdvtolf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vozexqmy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcvtmsib.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nowgkdpu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2srbaetvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmtwxoy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2plnfsapn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rrwsxbub.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2murnxrpf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lyzwwgel.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ponbfkrw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vusghzhg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zgnuennp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bdgixiia.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lczhhsja.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xiamjiqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qliraudw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgrjgvjj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqgvmuda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vreomwun.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dfhwffsf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wbcxhswv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lnhetmop.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2teynkwkm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifajnvio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pfmslxzr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mzlccmwv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gablhtsk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2biqvwcli.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nydnxyjh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2seqiobev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxvusyat.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2saydprsa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxrzbmbz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jycuevhc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2blldtdmr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mepxefyh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzufyita.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrdzaewf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpvoolat.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvaqox.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvqmsirr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otbbvnxg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrjyxqpj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mplvvdjw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfmvspz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2amjxpevu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tlaihrjp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kbgalccw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecnhitpl.html


<!-- 参考信息 -->