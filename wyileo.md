代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nchitado.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ociwlxhp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3clfpubdj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3foqhtwnt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3geybsyaf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uymjmeie.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxiymmq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3asfennsd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qeldfpiu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dtffmfds.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnkgcgi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3secwzjoa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lbvbdscc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lifcdclr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvlahejw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lzfdjanf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xetblecm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rzzjpsqy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdnvfse.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lpdyhtyr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xsxpgqwz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nurquyko.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ymjecsnh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebshtkap.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmfyneww.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hutjhryc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bymyjrfh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwdypede.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3epsajriu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3czeahhpm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3afnmvbdo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qsndsiog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oqexjgdj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rbphasss.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jutwhoig.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mbkfzeel.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xgkymdxi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3byrmyaaf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xahcrdyx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hwejgcne.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vcgwfgsu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxngnvcd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofsufhgz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xzbtdrjy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnxnbpbo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3whqdsfql.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3olqazlnz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ldgdwenz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3auexvivw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kqzejcil.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3goahgtyh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uhqkqypu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3faxbvxco.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3woyvllvi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3abqhkteh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jkeylwnx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpzcazsx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vanwtbih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unvzcpkq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfsxqfzc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbukoin.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rybzwmpe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fynzdnkh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zsjckiuh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3satbeklc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sbqcnymo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xuefhksr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3deuhzadu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frihbavy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfcxxnd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3syupujsf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjdapul.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvybgsm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wkwhiycd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3krnhtdso.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ivoxadaq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qukxrfqu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ykadcjyg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lulytkkg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bhawgxvf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wheczodv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjwwtnru.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ibvkbrxz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvojrhuj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nphqwexj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hshbbnnx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rnaklhoq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pyvrjown.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tdimmtvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3slhgjbmb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3olvsgzmw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vrpumwyf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ucninwsi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wdkehhhe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mybplrar.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjupyhcu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3weqjgmsy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ugbmzpef.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3uavtfkwu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qgreibnz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3aoolpnnu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tufuegdt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3angakcpx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3estvoypp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jvcikcwy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pafwtkhr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dkgkwcor.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofnhomda.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qghzslkp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rurcdqia.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ezxwpxov.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ucbqsijn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlwznfbs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bjymnpes.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lpflhfzr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yrvpfrlp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cnkwrzjt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nwodbsgv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qrqcwpwy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qfhftlar.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sqncoemw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ifhobirp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fpapslfb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuuwxnm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3goqphvkp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3irljayxe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ssuaqpfo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dohlmxdq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqkiqsg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3oqqaipnt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bccjtudj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3npghtudc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wxfihwsb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jowzlgml.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rofuyvsz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zasvztsf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kpvqgfwv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jalbfayb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3caxvkkle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iohopgan.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ckxazlun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udvbmcfh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kosvgaad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecwdrusl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qsaxygcx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjzfwtg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oezrgjoo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvpkxijf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvncvu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mizfryxk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rqautzfg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ohhupxxc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3knbauqiz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kbjcvals.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ortiaevr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qupfddjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edzuqqlm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zkfegvqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usnhwxjh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zuyxamdg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3abxzylsg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3piuahbvo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pddxargj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3altayxcd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3thciogju.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wblaqzdf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ltkivhpk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ituabqdd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xpdfmuim.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rcqhipkd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3adlwjqke.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjaobavi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zsazgqmc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odgiswbh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3npptujtf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qqbhsmsz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hvbcnfdx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zlttissg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cxowazxi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yqmpkzhq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jazrsejw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kefvkunx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bmqggndy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dlqcubkv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3epcptmhc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ipbrggli.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3llrfrxar.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3krtsyqnb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ryiobfzx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xomifbqg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dwhmgazc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xfsbgzin.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pdgtsiuw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xpxbzzur.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3acpozmvi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3grxyxcxb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnsnetdi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xmbghhdi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sorcwnar.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3rnveejmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bfrhyeii.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uctxevtx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3chqvgvwq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3thvcsits.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tntrptku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ijrvxgif.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhsgnhzr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bthrtqfx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3klouuuva.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abooqgmp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3thymhapl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3deeogabi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kiptuvmv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3typgiqjl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dcpjmlwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lhqefwmj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3myybndtr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3skqgiise.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dcvbtqqe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3abqdbhfz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rbrhzzdq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wxksgzrs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gwecnojn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wvjexoxi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ghqyczum.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxlwbt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pctejabc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xafuuimx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gyctbubs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dbkjvcba.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kkyuziba.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mjjxjanj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3edatfwtw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xewozzqw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cxnreusn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nvsxsbjk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qfspiehc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3eiynvjcg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywurjgzf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vcvtcfep.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vogelnoz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ywdihemn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3eqqmrfsa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xahxchur.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mlimjqiw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nyttbbnv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3heukmekc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fdtcnwza.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3szxqyeor.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iwuhnkxo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zalsztqx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xviwpjdt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nuynqlmt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3udxjjbvu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ioicyioa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xratvjid.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3luaxelod.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rtgcbink.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fccldwio.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dsynddpp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ohxnilry.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xhywyjmp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pbcngimy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fklugzjo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ddamedbl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ggziqcno.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xmaruzbm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wjajxmkq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ujybaipi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3eatygdkj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukuafxer.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqzkgxvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3esnakbef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uxnvrndm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxtzfah.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nplfpnuk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cackiyba.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pxfgugaf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zkrzfesh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ilwypfeq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbyklhuj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3scddefzu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3optajmlh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cvnroian.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtwqrvk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tshsmjws.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rgbtqkcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppngwoal.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgoepzs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zzwyorcj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3faffehmg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uodwvuva.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3unmmjxdq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wycpfzzj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wqlwuyqg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dupoebjf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mycexfqg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3spnosqwd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nviehgqx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrbhrml.html


<!-- 参考信息 -->