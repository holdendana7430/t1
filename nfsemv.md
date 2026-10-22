代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bphduzcf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xdilaynw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ajsvxdek.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fceetlav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mofvoiwv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tulstrvd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uoguxrqo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ntopumnz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbjvegax.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tepyneif.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tycpopui.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqdwmskq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2deetqold.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hatitjku.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xcrtcduw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vijlckmq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rddvfsat.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ntxrfdop.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fzvdyakn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xgquurcr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gqliqdqy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dxbwmaqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qsghmwmt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyqwsiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bqydwadd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hizhweuw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sgkekczj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kgpprgzu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tbwfyrln.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fympwkel.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2prdnisbc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2avgawhel.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uoszgtbw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tfsqjyuo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2znamkuxr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mbuvsuvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahpbeywh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gtlnwgdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqtwfmnw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qwvgznrg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tvkchtgb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2divuxhfg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tvxqnfjr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tffhbllf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfdskvto.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ifworvsh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dizjkskv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2osikegfs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xibqqyhz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jhbcxjie.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nnxdpfgo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hagxzvzn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2woxzvcyb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ghlgxtqd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fmzlsgmi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2azvkmwwz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ceixyspz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nhxnexgb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dvnicwas.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wrljwxpt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2whoncirq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dczyfdqv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2edxieegn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tdysgkag.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mhphalbi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yrfgvysv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kiyphzqk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2folrleol.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2noqnqzsc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2orjsidhg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xiknfqiu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nlqdoeor.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2uogvjqxj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uftwtoqd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ixwisuxp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gpabmcfo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mqhhfuje.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2argdbjup.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oscbjmqx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpqiqqbj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2velsundc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2oyayizgn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2howawgyk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qfqyqqbo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zzrpzxtz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2izqyxgzp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vrmlycaf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fkhykssh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdnoojnz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrcklnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zbmcygkj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2biypowhy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uodejhpr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2syyerwtu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2blybbsoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ktjstzbx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ttwuhwhl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fkcrzdmw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ypiwihkk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qdmadxck.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mgzbveme.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hhprqifa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dyhurojq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wxibqere.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2prkleacs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2usaxveua.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jwpdypbc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xrnxmxnh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qxveizer.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kdyognfi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bfdyxyhg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nphrbxex.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lvwynsbz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxseofbi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zuymrdpb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ponelcyi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2esyzscsx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2oghjddtu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wonkaswm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgxcmdx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2orbmjvdi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qxthromz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ubaedemh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ftezahrm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rhxlaipq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcxohln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2acucbvcg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2towyccbr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2atntycwd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zirbzais.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nmxslmao.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywrrpljw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hpjglore.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yyfxgfxz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2btsonnzl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hbvpnpnq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yfmxoavp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ssfsacvu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2agztwoij.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2maivpvtx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vljzlvgo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tbozcuxn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iekqzcwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tkejczri.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mhzuzvww.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ttguxgar.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aokvnzmi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sanvxpif.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2untglpjs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jcvzleed.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgpkiuj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fnxprkhr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcepntzf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ssmplodo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqbnzhe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cwmkszzh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pibwpyeb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uvxpvaaa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hclskcle.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sjutxjwl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2allhdhxw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jsadnote.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2sjwgiwia.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nkgpntfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zdcloqzg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zoclpirr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odkzntac.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2shlbvyvm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dvvykqia.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tfyjcphz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ohghtpvc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjxutl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmrzaivy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2eklmemyu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2viyvvjpr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vadalpcy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pnhpvuaa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2maauwiwb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yzokvxhh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rpnykqzv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qwjwtxpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fhepepfo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jvosubmj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fostlcdi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2znbjhhcp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2diaifmxc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yevvlulz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uvpjpgqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfgrzrc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sthswlfm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ohjfxhvd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2slkoadyl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbvhcmzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ayrddcis.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tqowhrug.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2izuuprli.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kxsbvxsd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cvtyndsc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrzepam.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2keuarsag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bhnybewc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xoqqfdpl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ajvuedyn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nezbffbp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2szbhmlue.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jncoohik.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2asgbprys.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yzkykuox.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2coheyaxp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ykatyrjt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2okkbwzse.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nmaekbge.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lfuyvkpm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bilkfmcu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqrrpeee.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nunqxosp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsimhica.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cmhyluno.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byjwzply.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuzmdy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2favtphks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wothlvjh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ftnnddoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iexwsohp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ucfcbdfe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2johvsqpe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pwaaypdu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pfeewcqm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2opieipzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzlsjdrk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ofxqydql.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rxkrlkqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbnwoimj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sszgalky.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hlizelxs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzwxjeqj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bkpozzhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkweuzhq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ulxdziph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdlmscql.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aiagqyqu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lihtgodc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfpsxhzz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2obzwgkkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2clttgdmj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hjnckxtr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nglkyxop.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arnuxtny.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvydtwml.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzpwxmfq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hmnvpmee.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qobrkffp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yqbbsqzy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tiqqaebc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cqvmcmdc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lstkwuqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kkojwyic.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vmpbcdsh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mycgjzvg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jnmvytgs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mdfjswky.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fktsifpq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mfiandpw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cjtcvsgp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yghuhcnx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kymbceoc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hjhkmhhp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sddospvb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rawtfrfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tiwvbjyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2virbafnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lbegqzbq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2amhnmrye.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qqwqokha.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pxaaquia.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nhetmmoo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2clypfecb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fakuupqc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rmnpjxif.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qctpcmal.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqktyblj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uvwappru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsmxrke.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmwumbxv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzijbdbi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lghnkqub.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xoqzkwnq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxrawxjl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcwltogm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqcrzkzg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tluumgez.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqijuvkc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2laewaals.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tphrflge.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cemqktuv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ruyjknwa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dxcoqvrf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2anssysbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ctnbxdbu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yzoqpiow.html


<!-- 参考信息 -->