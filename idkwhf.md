代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2irlwfwfn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2evkuuapo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drgwnrqs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pxjpiwop.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vylsjqqp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jikqgkgb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2flhvzzii.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qkgtiwmb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nedkqmkr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yfsxxsiv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hgnqqqjk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjvrvuxi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mobgwmou.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vgaidect.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zfervirh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxebdd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ccktjjtb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2uuulqtzq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zmajhdyp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdvlzqdc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpfmjtt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvtfizdh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fpjpappw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ypmxghwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xggeviwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bqkdwpvc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pjetkvzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qfvxtzpt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xirtvjnd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdidswn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tkufylfp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vqczvetd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jrxlvdsa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzidpqd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pycaxtie.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xahwfeey.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gsjefqlz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ekxdibbs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xqomzlvc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2igsbwqlu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vtfepurz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zbxxnkkl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rlmhhahg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ivtudxhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnxhzfya.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yavmoysb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhysnsbm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2btpsncym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2evawnzzd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cdwiofji.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lmqishge.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2imvejlsz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cgvyzzkh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rcpsfduv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hpayaxjt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2heulhvqs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2thtwzkbn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ikxrblcl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjclltqf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwynmniy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mbopsozy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zlhqswot.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxmgqheb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fvlhovqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zexwbowh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ywggjxsm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2famrvikc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mpkckqil.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nhxvczrw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2plnolhiy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nvfquaqj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2miskxqjg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kzqbhasb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kamkdzzv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pezmbqqe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2njgghbvg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2twgbremf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xpbhopsx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cebjfmde.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tvaqiubv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pudlfikh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rlpeeibg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxujbrre.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hyqzzrin.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cmgofgoo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2chbjppyp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfpuggnn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2serhhygl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2stxkayfw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cwbiwrzq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sbqqohgv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxdtuwg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tknntfgr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vybazshm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xwqhneby.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ayqrblgu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2njsyqodg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qsosivvb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2umvzujpl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lvvuuhyz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qamdjsuf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nofdnqol.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pzegqank.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rgvtaejd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lgehxtyf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pjrlpqzv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mnwcpxbr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axqxrbdw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qutshcnl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmndxoe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cxntnkyv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2eqeyhgjd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hpvbzvts.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oofbyuwd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuhuxu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2akaljehp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2egegvchq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2adagmpgs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2humhvbvn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2worlouzd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2edkijsef.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2stedxdnd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ljsatvmw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xukfeitl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwlbhtpl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qznnyrnt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qczzjefo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qsobyvnn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2owfjsyyo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gfulmbdx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jismkhog.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hdtdbzzq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cimqjooy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2frthmgvx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vsncqosz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2elotggij.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tefrfflf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxlfnsbf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dtsvvddr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2owwzssgd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dpzcymqk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mlfrluol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lviummrr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phzwjxzh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eavjqtxa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2skkmpvye.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2npphpzqi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hnnmvkje.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cvsfvuvw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pnuihqtd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzgztgoc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tdpmhjbr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2somcqwza.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aweecyew.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ysglzbim.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wgtdcwuu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qvddvzbe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqhgtqku.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzrsmxr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vumawcug.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuaolono.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xlwarmzj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hselbilm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pxqxgilg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jkidaobm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jicvhlpx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ddnlrpvd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ouqfapla.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfwxiil.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uduaqpre.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tuteaenk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkowaku.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkwfnkx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sbqzbunz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tornolcy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvyvhoru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqpjiei.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cwmchsrf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2extcreni.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmuisxii.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cqocjidi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfqevvq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pogfwmoo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqbqqhiu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2atjxgdgz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mhinzfal.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqbxjbf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2evxeaaru.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jszsigvq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qfwfgcbe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ajdrbqvo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2koigobub.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yebosjgz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2imnpkjbv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybszswva.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbyywywl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qjtihelm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bqoclacc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fngyedkv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yuvfkzpb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sxuslxlz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2taldnodi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wydhngxw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqtnjqa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2onhqdnij.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iixhwkau.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2puclqkjd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2umftkcoh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fouvfgsn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ohwvnslx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lbiffwyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rnuuphnh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bmiyvuwa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oukeiecm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dixenfmc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lkgvtzli.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ukblrplz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dlvmtihq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zaamodxa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sqamxxdg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cbtqsgon.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnpcyxpj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pnxpnwsj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asglbwsn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbhkyrrb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dnxqmojs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2canuxhws.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jhwmalbd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rfkoaxbm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ujkdtmtm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hrjbmmem.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kdqmbseb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2musqtktj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fwhgofog.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ejvsrdgi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pvnqgyca.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qyjglbqj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lwrbwhei.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dtpmdcji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cvhxqjez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gmrtexeh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hukqozei.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sqocqkkl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyqsrukc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xvwmzlxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdnshany.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2htcbgcog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uribjyvn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcxrgxfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zjbdgubd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2exxouskf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lfonqdpc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qazxbidh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tknlfbzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2srzmbbun.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zuaksyfm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2taifioac.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2plosdqdd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ikucdwnh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eserqvzm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ojpgatpm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yxlkmxam.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yfdtigri.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dfbrvcrt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bvqrefou.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rirnhqww.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hzayypto.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cronstzw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ydigasxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gzdkdinr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mpuzskju.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zswnjddc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jekakbld.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jwebhimy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mcxoghcg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xgnqwezq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lyvdibgy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zlaryfwf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pztvcvwf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kmnbcbgf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gafnukhx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yufrthzn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2evaqvvkw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ejmcgjat.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2aseqtirk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2flcryxgr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pmfwrvvr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xspeupwo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmviqdda.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sgizmbrw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lutupngi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxttppqj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltyzqiru.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jpjpwjdz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jovbcjgn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcororxx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcjccoir.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uexrzvzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wnlqxdgb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2droezfkp.html


<!-- 参考信息 -->