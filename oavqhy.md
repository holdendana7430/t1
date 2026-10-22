代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pvbmomxv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2snummzzo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztciolrq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pzgzjvca.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hwnrxgqr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evklwfuw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gziciuuf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gwfejsne.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2olozomvt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfusjmhe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijyqwqvy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsjevzuj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rwypyywp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jxqqjwvi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qwddzgnx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rncqzwzr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jfilygdc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rmyujnfw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dqpzbnay.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ktdetvuc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzjbxoim.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sfnxnzcs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eiltvwss.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzufmrqt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hlvgzjyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qajsbdrk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2thzoahdr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2buijagkm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vicfhjcm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vhmdmlfy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nifyojym.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wouccmkr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oprnyfep.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2axwkcnth.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhstmlg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wjoxtwnc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vldiecdf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2knvtsjig.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yklubbnx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zrlgsdgt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ncdlfroz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hkwnpopz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qsmgxtxy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2inbnuyju.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwlovst.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkpsrdek.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mxltsugz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btkkrpje.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yicvjttj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwlurgq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dklatxqt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wppexcxy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qtujglzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2totwgdgw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nupqplzx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gnysxfpa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wtshoufp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jjehbjea.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knmbtbip.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2omdrufvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rllidtfl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hpxlnnfs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2woalwxws.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pszmlray.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fegosydv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2grjtcjsh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wujxdgvx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cxwupgzh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tsxhqeay.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mqqkytbw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlxydztp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjxjgwn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kktuhwky.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2agmufwuj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlmplkj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zjxrbeaa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yipqmhtw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pyqhlwqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvjfvtay.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yuovlcdy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yejoyxjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ntqoxsru.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2reslkqpr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zdpqqdrs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qosqekqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vehbkkpv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bgiohkoy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aiaoszqx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xevxrqmf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2povjmzjf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nzvebxbp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ujpqywbn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nfyzjgcm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fpikvgbu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtnigar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkevatm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bixjwhyc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gbulxasp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rraxupdh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkcwyspj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2osopvgye.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ouaymgfr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bgvnsqki.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mmhtytgu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2orotrtoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ycecyuxf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vkripbqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyjjvvl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xyhrobhr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vrbjfkou.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2adbwrzdu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nkgtwlig.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nmubbiqu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lummtdpg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stgfsfjg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fztjjqtw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gvbfktwb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xclnxpiv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2idhsffgn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ezadthfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgkqoqsv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eubtdrxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxsyglfi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blbjgbxy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kgqtfnyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2scocnigy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ugcvnjzj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fohktixi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2szccbizn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zeqdlbcd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dcenvpqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jdqnxoxa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2daxylyxq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2snudqiks.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ocosjlqr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ylducqze.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kakupslm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2edaehmbg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uleptavc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mhficrdt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wyibxgnj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uymipvls.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pnghgzuz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gfmdccgb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yjwmxbpz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sspefagc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjyrals.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kndzkffa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2roqcftfr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jxieucuh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nuddmpmt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ubenjmzg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bnaujpuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nktjqdvp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fmhwnpuy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2geiouwus.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qdebbyoa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gczkrzpb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gbhsexhg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ixdjponw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bhpiyzid.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vuioqjka.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nhxrnazu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bovglwxt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dounhyep.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dopdznnr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wngqvqte.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rdhzpnlb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cfzdydfm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ramwvsqd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vggawnin.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmyngcc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2amxjfqix.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cmdpyjtv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2znczllne.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2awfnprus.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ngkceyzp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xtezxsbw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ghkyygqc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdrmsuyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2teyiiwks.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zczgcimf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uvawkqmz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmofmwbx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2psfaudov.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnjyicp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xlmywlik.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjvubkn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lulyjdno.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aniojzqt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vporiisq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgfnfo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tbslaeqj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bxsfbqwx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kvjcvyou.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yznidsfm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxrhichs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yuyaankc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2babbniuq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2upnrslnx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cmjcjkpk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kdqmjffu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qoubtcvg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qbeysjvh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jrhlsmbm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iikbhthd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wkrmntfe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2swkatywy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xxhnpcld.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jqcvjrap.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2acvnmilt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jjonjprq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ozzgofuk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktjfivfe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hsokvarc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbenbzts.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pihxvxmj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2breevflm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xghbmsaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2meyoqxik.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2spetnvsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tbidnnuk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nmfsxkox.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bvfquyps.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2frmyagei.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nfnhxrxa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbtidgfy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sxsdcgjl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pjcaoxhq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vwsejdas.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ykdhznlh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uskaluuy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tjihdqic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pubrdeml.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrtlyykd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktltbwsn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lqnryqar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2blvuuewy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oogawjtt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffmjtbcy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kwdbusln.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wbbtpive.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hqkqrihl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsuxvry.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nhaikgnp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2delbvsfu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bzscksxa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cwubhjix.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2igwdirev.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yjntigkx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xevdtidf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rxxmkmok.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nscqklbl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ywzemfnj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ttltmlzd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erssigru.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvggvnlf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rbonfbib.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xanviprc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2saiwmrnp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzirhka.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aropvrus.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2asbenhpx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tltlpzfg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ihmbwrwx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lztlenwq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tbklmtxb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ppkyermm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rnbpujyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aekkfehj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cddwuffo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lcgqofyo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jkerozry.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2imandsdd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2njxgirow.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ewfjkxsm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zlmpqocd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lypdumlc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ijloypvj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bxakaqrz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sckvqkea.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vzeuglny.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iavawpjv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fsqveeag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wimkuapt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jvbxknkg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hhczcrah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvutvbmi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ponlhqrb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iohzjdzd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wgkpfwgo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xvlvecja.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gpxqhgul.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wwatqnhj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bbeplujr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ckezjcbj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2znttpfbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivbwrmfl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmacbgmt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqzjtrjo.html


<!-- 参考信息 -->