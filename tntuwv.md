代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jtrqqxyh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uoudtvrl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2quqtzrer.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pndnaqxq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2amnwkrzr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mavayryl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jtyhgylc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2usrddoav.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vwoyfynr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnptxntq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfixdthl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fhetymst.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wtyehdgs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2spxinnvl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lgaxzjar.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rodhzvpq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2piytbkuf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lseylxnp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfsbgkgk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2logzjrlz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lysyjygh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qqggztvf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zmnaufww.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bpfnbbtd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zwteqbvr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2becmqdnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mpnkkfrh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2khdwhyys.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yubukjvg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywgvuvxy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bkbzpanl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sunmtmcz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vbpubeql.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nvzvsllv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2uyzdvjya.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlfpmhc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxcssfbn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xwxlbdln.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ipeaocmr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2giqqkyob.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vopwsljt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mucjeyfu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vktcjkal.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wdfzdvoq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2iakfzjck.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zjelaufw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2smeqcugq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bbpvaibi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mroozeya.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bhshzpse.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yuofoine.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dwraxaac.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2aimmwhbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clwqfkgr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vabovabm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2gumyvfdq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xiufvgab.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pehpyate.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2izuwptao.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qlhdjqre.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hrbmwmty.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tgvvulfz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sxtvxkjr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dryyqzvm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fosgmvmy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ohlfxhgc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jtakxszv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iwopefsb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dgdisjhz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tegzmfzr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2shxbwier.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uerxbdzd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hmojdwzo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uzfrzafe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmkuarya.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wwismhvl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjgzzezt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlpwcbo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2safzwenz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lnnhlmsp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eruywyzx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xwgcnzhu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfmwzmjx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2djmarndy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vifzkpsq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uoowfglt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rqirwonn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qerjhxqu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2aheuuyym.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lottuttv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xpcctieo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ohwdelod.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vtizwxme.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vzummefv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mziwweya.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uibstduq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pqhbhpnm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ucnqyzii.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ueacarie.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eyyobwdv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqkrdvnk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wljgozcj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wdmchxej.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cyzblqvk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xxmhvdpw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xifslbjy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wbhhgcul.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zkxwbkvr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ojoviork.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2zzxuylcd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhfsebcr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltsnqtlp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2stxerumi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hkgespwq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hpafctjf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ldqldvct.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2glxnfebz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jwrpcgle.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ydgtlswr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fgxffohw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pyloxomj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ciyjanpt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2awnqhbwk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zmelajjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twqhwwcm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rhrsttkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndntuked.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kbunqxno.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qowhipez.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2epzjpbpq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lghjwwix.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zhqjyjks.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zxvhkfsz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jclpdawi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fzuysdrd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohbvkpcz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gsuvfovj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2udsgmziq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2boxqrdtt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgfocqcb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ptlnxruq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dahuhrat.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jwuxltqh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pfavsqfu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pcrtvlon.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xrlpcgtm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dlrybmdz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zjnbuklt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pfenlsvw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bjdvzpwv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wcxbfrky.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gfrpifty.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2buavvazo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2suzvvcah.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2emzknsrq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mbhyhlxp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nqfqxqrm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2duqblrrc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fulxdxhq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eqdiesxm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2grjhdumx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uyutzwjd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tgeoeahz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tiybedxp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tbwibejw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pkvcyout.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2apkgzxnc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vkzpxevh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vbiybqqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wrdhvpxi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gfqyzjfi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vjsokhmz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lkjxbvyt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxxrqwh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kszntlxu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwhmgxje.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcigxvem.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cesuievs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gihghmss.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wxxldizg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2knrzvphm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yxotdjyn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pqlvkawt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mpxhjtxa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vkqoeugp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hufrgzfj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ficvhcyl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kvxtbgzx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tfiwtsil.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yvreifry.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hkgllgca.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ljltwuer.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2trzkvpco.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2azkpzaxh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xshyybgs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xxijhlio.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ketndjbw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qclyigwo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ixcrfxbg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2aecxxjpb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgedyemz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zfpybapk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lqsjtjtz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovmcwqxw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wvzpotna.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sypquyuy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2liamqqvs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eivpgzat.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fnrrzqmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hmpepwog.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tgmpgdzh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kdbouwem.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zaadgfeg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnxhwta.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tsbeqcqq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yavuwvpa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bmbolezm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2btpuzsri.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oaltqdix.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2slztwzwj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evyefopv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwvjvlqv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2btymwraz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gpdcukiw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pbvbspvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2riaahkhl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rlcmjawf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tlycnlbz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ftcczfdd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qmqgqwqv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwkhlaco.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2joknmhjc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mgqaydye.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jamhvayf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vzaoqsvl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jknmgelw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qweylgsu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aihtcgpr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaovabll.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mnjkewty.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwuxudqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eegekilp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fsixkcbh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2grwodydu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dmbqjzhy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zemikyam.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2prnarqsf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpdbrcb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgaktcm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvysxzw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nnlyomud.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ylokpjjr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2apcswhmx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2omksmvkr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmxygqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssanivjt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qoraiizb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2whavzyeb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fuhnuatm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zestddkz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpydywvu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cfljzchm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2myrzodja.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxrmbrfn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jxgovsst.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fqlfepqv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2msvblubc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mkwbazqm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wozuqaes.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yvoblikt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2idjubvri.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jcstfzhi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dfejfmga.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pzmeescx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2roohymbc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2umracnye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kyhwbjeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hjugsfhh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bwwburpj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wdxrbgyu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sublvtbo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ovlxhwcz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jxrzbuqt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivztqxzg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cncbjijm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjbwmay.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2onznbayw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekjzkfom.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2digqzkhy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2usssgszp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ahvmtotj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bmonyrbl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwlutyy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2erhrunsj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uubiittx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mkakecqz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2pcysqzpr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gpnilrpe.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qfxepwuy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ifvvybfp.html


<!-- 参考信息 -->