代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lvbyttgz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ttcdcsoj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bmiylpvc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gkqmlsdu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mscnirem.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2odgiidbk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qoasbito.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yjlnxdxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mwjawvfz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qmlyodgh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vozseljf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2bitahchi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqgxjzh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mqngvgqj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jmcawyzn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2todklplq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mclizvvj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nzdprlts.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kzyaurhq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ilyenmgz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2efxhnwpb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kctibddv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zxzrlnpi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnedctyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zyifhegu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ukzwnqlw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jworerkb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oxrxseuh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mlviiiio.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dgkkgjjw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2loswfnnp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fvhzezyx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2caiyazws.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qgsytxov.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2opieazrh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gjqmixwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agmzrkaq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wyqwdcxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axcmbzbz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2govzoqff.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bfxciral.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lezxfhfz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rmgfbrlz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bjkxhwsr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ixyjpvxc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fraybyla.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tcyusjkn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nebaszqf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhwjzlhi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wayeqihj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qymfnlvy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mwyqhdhc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpuzbil.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbawtts.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofiadmch.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ketebxgr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lswotybd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nsqlxnik.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jpxbyahi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltbheuqx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wijueqij.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jraouvmu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsvznnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qynwfnhr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fufercue.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qeybnilf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2odlvqrvc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2odgmnegd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dqxzqirr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jthpcmfx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oeszmjit.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2onvfaurx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ckicwrnr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tuokbvou.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2obylpfpf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gcpnmnki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ojumxape.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kndeteiy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tdrcolvi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2iljhendt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ledkbfqu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xiljfvja.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mbkaejtd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rfjjrkhh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2grdhsblp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkesnjil.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eakwplts.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kdfivyvt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eixprntn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xntvkanb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rwspeunn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tfxpduld.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rrhutyeu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2phpafboj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2siiibowj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfkgcfwd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dguwosqn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jebapcoe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lwfzqzhg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cmxvresg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ltxvetwo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hvmkmelv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xvurpgji.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rucqjgvv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xechnkxh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lgtieatw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bvivvpfa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pbjnzcqg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bfxczhcx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dfqpuiow.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lcskgglu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gibeflei.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqzlvgz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bzuqsccq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ontdsesh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2axesjlws.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qyvowybf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2axekgmrl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rbnrdxvf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hdxvytxq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wvftwbtc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bevmhygh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dlphohkf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ywiqjwse.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gigytaoq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2khckskrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nhuhppjd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2llbiebru.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yfybvazc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tfkfjnoc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pwiadlim.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kefxsnns.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2luwyovnd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tqkingff.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yuoaswup.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ovfhlkic.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ozryskez.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gqmawefl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uqenhnrx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2atfqnomc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2knmnuzat.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cugsdwpy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rascfgsy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zdegsoad.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yywvoqfe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yvnveciu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ldmytahe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2avspcrvd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gdtqngyx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lrpqlcon.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drekfjri.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hvogradb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ailiadsy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2bzgbxdha.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2yqkzoxpn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zkuvsxbj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dvdywffj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dbkdtrqh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efyqtatc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jawijvmt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fugpfuau.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gxeqrmfu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2oiytcwmm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xthkfzem.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2syavixho.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lutpqtvm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2krqilhxu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ldacbukc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bckqlikr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2leactsei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lgogwoqj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slmnqqky.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2waxerupb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrilwzaw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lunogybt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylkpzymk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bpgydsop.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2odzumklz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vrxqekzh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2txewdvjb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2huchbrup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2njyafpvs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gatmimmp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2soataric.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mjcpxixg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vlwkfihg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2banubsdc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pnksuyei.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nrdyqpwy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bjxdregh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2korbkpme.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bzyrvacg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pgcolizs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gcjtwxmp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2edwxkdxs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fvjwbene.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vmegkykc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sssgnmaa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mxwqgybe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhimzipd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2olrjqied.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tuixwfzb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pmmofqhe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2frwcgaos.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhieqznz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zshwmkkn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzuqyyi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sxgaxxgi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bmxrotsf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wqzznwri.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fdditsyq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xvaamsid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ecqodbyn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cxcrgvvg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwmfyude.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rgelpsti.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyzlavez.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fuaukqnx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqgbolge.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2raqezoke.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aeohqtjd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ycewsxom.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2geywrpsd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lwcetnzl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pmlpmjiv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ryjvdytb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kveiruzt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gbeuyeme.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ccjhpafe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wiziwypf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmswpk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2htzedgrc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dugafahc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hwuobbws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fsebiiyb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cpobmmqa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tpizdumv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miazcjvv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vaokfxqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlxzjtfd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2srhkvxna.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zohhewhy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2viqmcuvj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2irhweehz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2acyyrkrs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tvvcshhr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xzttqgxe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vevjizug.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2puwsydpl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2aetofwtr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nzmnnfmz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2detsjhzc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dmuipxbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gmobzruw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpmqiln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbfgwpnd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2szeqehpw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlopzwwp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hzyhoumc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2brjsssuq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oshkmqcz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yckmfazk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wxdqofby.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qeucnblg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2enkmvxnr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2axkqqwlp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aqiebboq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvehmdbr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zrteprfc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pzasbrgn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jciczuxt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2flxvahfu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmrrygr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ikaaeuzg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zwhtkwiz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2cqhpfdba.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ztgcnpqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vnzpwthf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vshrxygl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdznfsmg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdnauozx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddhjwtft.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vawbtnda.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2puhkcfbd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhzrvfat.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qqhzxtbb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mspugeat.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sleunmlr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdxdilia.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mosnkiut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fenecehg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnnpbkvp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfjlzabj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmccrwli.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bgbqziyc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eepddcyp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2btllprqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vxiswkze.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ohuudfdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fyjvkphi.html


<!-- 参考信息 -->