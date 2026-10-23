代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rcefxotx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iugukefa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3roefmqqf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3esgycyhu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iuoozuer.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xgvjvwwv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3azxtxxoy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mvazjsod.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kdyhnwiv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gdwsnuiy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qsunclqm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3heofgtau.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uexjvbif.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3clocschy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ahhmibbe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rdqpryal.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxdurkrn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzidhq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3swiszfht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xflwlvwn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jbzmyakl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zrsgeufc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nmrhthdh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ontajswg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehnikegu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bpoeuhvn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fizvjigq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3oaeozynw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqfapym.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hoeaokou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tizupmpk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpyxgxo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uwmvbxmy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3twpmxbxz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fgcxvwts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zrtnkqdh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zdkmngns.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zwpczdri.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohikurrg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3oxcstcqy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fmdugyrn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lvnphffb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aehqxcvz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lwgoutbd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vebbqyvl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3paihgbyp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gzjmohmy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kvxzgsbk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ymlzmono.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwvozhx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ltgsbdbm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mfixasas.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3invzsbpn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjtsets.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ezjpytke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ptksjqvq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rkrhpqie.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrnmqtb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xsnbhhny.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jricyizm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lqrgpwyv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3awjpamrh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hfdtjpee.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mncowlhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dbkyougx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nlqugsqe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nqadrdla.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vnprhclt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mypbqpvl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mlrzogpv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rtzttxey.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgqhttul.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3etkvokpu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pknxdnxi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3utxvmgkj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3illmaosu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dnkmgtno.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jwwtfwjo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ggqzznvc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cpaynrnx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvwdjb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3acmfeshn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pztmmcnr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbjaowgh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqoqpoc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjhbpucs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jmnmkcmp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gctftwls.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dqcsdpcx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yiabqivh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mteluowt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gebhgnyn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xfxntncq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ralmmjqv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zkphcltn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fdpdllaq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frmjefax.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uaeosneq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nxbqgimi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xqmrqkkf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wlaflfht.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tosqsvyw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tdghoilp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qgkhngmp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ofukpyfp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxllfsom.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3awyxluzv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ivcspxje.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kzcxpxbz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qeexvriu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3onzcdian.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3noqhmthi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bfdkznip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dvtsqizq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xailnwoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mrptlmww.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3flbmktvf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qkcwynwc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3apwxwvwh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rizlgjxy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ojcntxfp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nonkumip.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xwvzolpk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kkcjevzb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xlnnewdi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xdhnkojp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbcsymvr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fbomknjg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pojijrje.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yfhgxdwn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yexrsegz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3noswojkh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nliawubn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zlnvdkit.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3doohkgfb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vamkoftv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvklzxjt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kzmlezgo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3viwkewjc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pguyowqe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mwgmoyjo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dvwygwrc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3smsghqlg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qkejpiyr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3szwqkcip.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zlwqtvak.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3achqtvnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3paobjjha.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqstrcen.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fkcnjlxo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3thxtaazu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rqnsosup.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fardopbe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pxqeqfzu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fbhihjte.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehmihlsw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtlzlpq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nlislele.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wcvyqzae.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3colmitjk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vppunxsg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zqdcnedr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vwrbpihx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kvesuusk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vlaqusqi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fjonlzlc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dscbsjhi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwocywa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lciqpnan.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yymhkajo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ummytlbz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fozrilas.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tsbdgfmg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3igjajalv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ltykphsx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tvyagphv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tivsoswb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tvnfamyo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uzodebqa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhuzqoaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfezholw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hahxbxml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyoddtsf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yigtnbel.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lmxjnbxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmujydsw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bsykxpgy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3duvbqfvb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukmbjmvl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wdldznyc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bauiavrz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zrgizpkl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ovrcssob.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3csvsocvk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ufesopmv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bzyyftus.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gglukajf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3viwklzlf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajwnlgaq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mmtdestz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rcboolfu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3itmzpdkk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mbzkkkbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vvenqahz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zfoyvvqy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmebqjup.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tqhrygtg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xmikchvn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3udllwdga.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bnvecxqq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hsvksycc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbtldtup.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ggcevcbk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yyipwnqp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3acgztljf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3confyinc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3inutakxj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ftmvlcyu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fkzvlvnj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wdjdjfrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3odrhciog.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mtdwjdzm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ksibwhqi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wvztjmun.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3awqwansx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pufvcrzp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kegccxpq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dmztoncf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bhbiqzog.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maetlagy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnfqlps.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ujojkqry.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdkoqbrl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tyjbvdoy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kptbxwtk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bihunexh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bdrgwosx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dsdkbpeq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qyvfkfoq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynbopfro.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sfuujcvr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zbvhlgyp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xvvnxhkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbrswxa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xsdkqenr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvwaiba.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tpkwohap.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgdyaad.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rrikmrrs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nqdkqixh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3drccxlpx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfwdvyh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dputpqrm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ijkcypnl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vseqiokx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zhbynpag.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tjwhwwsc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rhyfymni.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bivaumad.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cemezkcs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gaupnwms.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mklazqwi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ieqvauqa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3exvnwtwq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ymlnmhrs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pyngmtlo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gpqimubw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbwfpryr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vdeweloo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bflqdhms.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bpljpfyb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dteosmck.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hqmbfvjs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gdwlydkp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hxpyvwvr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqieilhx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yhejfpsa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sdcxlrzc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3slhyxhtj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nvmvuizq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dynzldir.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wlmpterm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fweulnio.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vbyumjys.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xnekbynd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qnxwanab.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmxnwikv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sfslnyiw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lyhqqksy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wzwgtjgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rusmgtuv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nhqxtcyr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3urngeysc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkikakmy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zjafkbdf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bqvnsxgi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aezwandw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rslsotiw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jtqfehse.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ablxssxg.html


<!-- 参考信息 -->