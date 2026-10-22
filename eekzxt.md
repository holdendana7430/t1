代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anphqqru.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ckdysyol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxdhxuej.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dkdybtda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tynfgllr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2foaenene.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qjctkrsl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ohvokiqg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lbdfbobi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2izfztlaq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ojdotwgp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofsuxqzc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dkjbzfwd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rhbcvxzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ltetzwcm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zdvxbrht.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wutiipgp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xkwkullj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnkxvmuh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fqhuutpo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vwdogqcy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lxpmgdhq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gqbydzhb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gujpyika.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtdpmuay.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xmmqtrdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmohkzut.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zkfuktfg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2idicrpfu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ptfjnush.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ordmhwfi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gtrhzwmo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2poagaznt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2snssvtrq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wpidxbrs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zttdweaq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmgkmaem.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fysmnmro.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2occssgpz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2klylkkkw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ykubwjpn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dhphyxmy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlctefrn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tbthhcyi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zrdjbebw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2epkvltmk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2kzbwbspp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lwjlumxs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vjebhedb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vbzfkiex.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qmxzyztc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tyzkyezz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zvwgxvjz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2itntrpxt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jhhdtets.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dmytyxod.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hmckrodj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrdnuhu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2opxndavm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oujzggjg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdxoojly.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ilolnysb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pskhbgoq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fisabiei.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wtbjqpig.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mlmghuyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aairxqax.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pnmokwsj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2natsjlwb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vmelutkl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ysldrmwp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mrdvtudj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mucflgwr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yluthfok.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mulbkpuo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pxyewuqc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frnwqbeg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ungtrjjc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvoxaezp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxqqxuwy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2upyobsiq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vsvuncdk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2remxzwpp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vurhtjuq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2emwpaxew.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bllyeadn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eekogdbq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tnkdcdwp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yajqvmeq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lfccdzlr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zktikntn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwdrvgs.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ijmmxvlh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sepzeveb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xosnjuqn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bulnczmb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lmanxdfa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfgsjdk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2seicftem.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rindsdvs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2adpncgrb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2geaeogpz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nxqiicbh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cxvgguia.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2glzrwgwy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxioxsrj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qgllsplh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2amaafeiz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2txddwrkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2izrdgnfr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kzrqpkgn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knqcixlp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qvauytej.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mpfupatx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dzcgjrcc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bucposxx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2clkcpmfy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2irpeabtf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2svubfkon.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkhocolz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2opzqrihm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2utizeioa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cvgfjbsq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cbpfqdwb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ppvfwbfq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmqxhg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fbtxdrxe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pxkigumj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kwweygck.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgoaztex.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2udafrrct.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2stwgqkfe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eupmsdwc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ldiboxdt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mggzugqo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ixtmagjz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jajsajsp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uvflbafa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vppkkgoa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyftatak.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mctawjdf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nxrhrdof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ryjcwimv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sblpbcdw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2czlfyuch.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdwbyfq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cqdzuivy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wxvntdjp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lcmqltat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cdpfdwzz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qgdvdnip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iesinces.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xaproymg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jqidpntu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nywjootg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2teqqbcnj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2naodyniv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gxyaqdzd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zvfcnjmv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvmmsd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joovrtgk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mffhahks.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2szhdtjli.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xcrcewno.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2goggkgpc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lxyumcud.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2scfqkyvj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oljubdhi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sxodrfyn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zmhfvatz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zpsmdtyi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2aqhuqhwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lbdmbukx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jnfvtfol.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nwtwygdt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhwesgf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rudlxdau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yopgduhl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zfvjdknl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2blrvtmlm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rtltzwgr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2luwdewvv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ywawdska.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gyztqhrk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zetzsmkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dakrnpea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fzeeituv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zimlhnqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nztquodh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2feeeguun.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yjxicizm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wgtsjznw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbdbroe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wcudfjaw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sjspoybu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvvdaa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jrxowkzs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2unqslxhy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rtgeltas.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwkmwz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xudzjxhl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zkisarpl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2svbcbsgv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibbplbnu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xadslxgw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gbngkwvy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnjuimta.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tntnjqkj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lyhtjcle.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iybwldnb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2brpqonaw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xmhbirtp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eecimjsq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2njdcxloq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnwxjbhm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jepuvood.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ptcdhlhj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2snhxaunb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2egijsije.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjnkbkrd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hdlfalmy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rzugwwzt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hfbuveor.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vtlwwpef.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vtfnakte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcgwnfdx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zzhlzktx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwdljtqq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfibqgzg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lkckcxny.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymvcdyof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2njtavnhk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yfcqhchc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxswzvlg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zfmnvslb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzxquzcl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdrlxpza.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jclyoqqf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2akyewxfl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2phpocolr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jplfezoc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjlmycaq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2joydanbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cnzfmgcs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2twwafwbr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlvqbac.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tvxfgawm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jhenxbyn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gbolhlpq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2abbwkhmr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ubxnzbzm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zosxlhph.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hfvantkg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2prtxnatx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vgpndfcx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qsnuwhbw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmxfswc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2izgzgvbu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2orzrvqqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwafwhwu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2saovlilz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xyajpapq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hlidtdmv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yykcxbgy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mdhodykw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2asqnbnie.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2viefhcck.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgjkektc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqbhvqho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jyuakqgr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwyagqi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrzisnan.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzqkmfnp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfzmweno.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkxxieqe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nmglvccn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmhcoijt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbesnkdx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbfclbuu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evimjwwy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrawerov.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mvbuifgp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rcipakum.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xqfulaxm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pgltwgpz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hffuokzd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ppdvvcxy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dhejkaiv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hqognhly.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2audvkoqh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kovlnfxd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mjgfxjoy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ikzthpyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbkieem.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubfsciow.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tpfuwgpj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2clwuumnj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2frgvuuoy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yvkhvujw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvswyb.html


<!-- 参考信息 -->