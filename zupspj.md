代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lbmllfmi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tqhcwwmp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pfhcowgg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fmajmbre.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ifpixwmk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dlpwlmha.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jdyjimwd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fivjznpu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2deoimitt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bgmridvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmqhfuak.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpkvcoap.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jjetrckp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vzbqhedz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mtypmlrg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lcuzhanu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2agyacgjx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pxuvzuja.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ojaxfpbo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ucmzantd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfyeqmjc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gwecqkjr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ncgpjsiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ydywbmpj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2knahycfw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gmjkefvb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zceqvznn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pudfpagh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2iywpfcvj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2iafhyvjj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2iruwaonh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tbrxbsfh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twtipgkm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hvngfysn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sqbaqled.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2teplmeek.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gayqxehb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfswsmh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2khynkyew.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ehlhfevg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hmxbodsc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ysexyzzu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bvikjlru.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ntxrpdqx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2weswrnht.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pgmkpgyc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vfszzmte.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rlpldlyd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xleytnhk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jykaqtiy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vnwoxsax.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wgepzwhx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2chrdiidj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bdjivjcv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ukgvhjrp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zbmriyib.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rlovwsze.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ivljqxnt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fngrgyey.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovzmgrbl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sexoujls.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvimbdc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2taadqtah.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qoqyuywk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbwlnqyz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ytitewll.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqvqpuxg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oyyoxgaz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jrtbkunj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2exmnaqzn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kpyytxag.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uuvtlrmb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vzcplrwd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2syruutzk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vwlobhmj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fvphyltl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smtakvdx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhsrhhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fheniytk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2morileui.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqwusyj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2toxmwbjd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aumefvro.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukvvvnzj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2irbqixwb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kzoyzlvt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sjzwmucq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rlrvlaym.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kfaoakmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vfpkcwby.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ncxonxbz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qklpaqbj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jnrnteuz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erhfnpoi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqstao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wzcfjsri.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ybllcpix.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2oknikoxf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pzembhki.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdfhbnzq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2odmppkhn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqovkqtw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rlftfirb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2icwrrvka.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qxpgfnro.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wwidkcwu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qpilzfud.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ehqsfbfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prgsodim.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rcedxpoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmxexxlw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mskswlei.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pnvhknnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kfvytfab.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jwvmsigq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2skwhlyrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbbdzpei.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bnyhhrmk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ggttgtrs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmdofycu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vzdjdekp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jxkrfkvp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oghsofvy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ouelfnyr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnsmxdqs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ymwnxobo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tiuunumc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gwmiparj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ksfpcgwj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xxazkgct.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iqqnetdg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nxehvxzv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hyvxowhm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2awahzzue.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vcqqgpuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gbdbypad.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zmoxwqmt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2utfumfqf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xgfjfrfi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mxaonfaa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tuijxtnu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ctfpmyko.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bfedswkl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hydgplle.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2keqxcild.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjqmdsk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xmjyxect.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qsfzryrp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntcdzblt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cxclyist.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ntbylztl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pmlaikpw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ypbeaaut.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nonkmzhn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iekulmnq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tubecesf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2plskjmzl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ptwnezyn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jjghuxvs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hilltrmn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkegvnpa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vbjghyaa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2areojsrv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ynpmgrdt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2amybogoh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kxvjkzxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gayhhfqv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ccsesvxz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zohkpjjo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vpnzqavm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ywklnojs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gmavpwar.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2illfpckj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zsunmhii.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uhmmlfif.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hagsjvrt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vjyhbsuu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zuvjqngt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mdiprfdx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oigzhuop.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wvizqzbd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2detnrrzl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dnewlpuz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fivqbxpr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wmtymzsf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eowxsdfv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ycscwvym.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dnhyzvcc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjbnyya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ubqdeqkh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zswmywmh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tzcdyoua.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dlayzlcx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2elauzdfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zfhjjsca.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pziwvxbq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2affxxdzm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hpivbbwz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqsxvkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2abwarjzv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pafukedv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2seouflwf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ttsslbol.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mackzaqx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ubckziwa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ivlwfjxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2eojpkbpn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ngmcisxc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qdkmowgr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uuwaxnbh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pklstlah.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vcegdhav.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2evwowchc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mafxqkyx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hnuhvwzg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cxlygula.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yuutjbyy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sfofxnhx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2famsajbq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehijkklp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2irdalrdk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vleivyod.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xrvbyskq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qeowprua.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsffwrlw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vjowxaik.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gkubasnq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wamrafvj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ssbuwrto.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2phhqhgwh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tmvoaprp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mzgnxxzw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2acllshln.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jgzxvqil.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ndofgcan.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kmnjaayo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qrtryrzf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2euqgfcdo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jjlrfcoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dwcakisq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lsjfctaq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xahpgeta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mxidmcwy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbbejlnp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhyobiuu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdsikpvl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pixzevjr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mttxirys.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wfnupmcj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lmymklva.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mjeildqt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzoojhh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2izxxlyka.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xodkfrbm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qxglzwrh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wdrhdyip.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bkybgqin.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pjnbsiwm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yykftnql.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mimrtbfh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vwskbhyb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wqtjaoul.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2axzylabc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2eylkrunb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ivnbhcmz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tbruddjw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zivyctmv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zotgoxyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pguzxvcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2idlgvexv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jweybybc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qukkdpsc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cfdpypru.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dqwutdrc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jarkiviz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkvtfafl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhmdxix.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqzjrng.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qvwyizvp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mhirlfld.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ygkjsisp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjeetk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lembzpud.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2asbgiplk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gdgmlduq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xifoipea.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mojemrsv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnjmngmy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sofazlnn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dntmtxep.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvuvybmp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qihzzshw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hirpwwnn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mgktktvy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kulpsiiz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2llhwelgl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dbmuxbla.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2thjqbfox.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tbwglfwi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tzwvekdo.html


<!-- 参考信息 -->