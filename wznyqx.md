代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vissdlkd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewlantmn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dfdzrtuo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qdfnqatm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qsuvgzft.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmqcgwsc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pwwqklju.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uhsdukcg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qiyffxmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wfgnpwpl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gverreyr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nhbiarpv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wmdvdqpl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2znwbtcbb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2usufzyor.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kbneties.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2axsmcwdp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2swxrifhd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tcacntkp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tirxxkxg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iaxcxnxy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dtihicom.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ouqmaqoe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pirswmsv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofduwcns.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2enkbvnpt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zseiwmot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qpfyzbch.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cngezpkk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mwtoqiwp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ahdtwqlb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2iwedfqec.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iioydbot.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mnvgmchv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tuziupxi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gmgpbifv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcrkqls.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kekugxtv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zxnzsfwl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ysmpczax.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xqyqlgbo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qdqkkuby.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nhagoftj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qsproiee.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2akazxzee.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mftjlwco.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihkbcmjz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kvflrcho.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ksaivjbx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2roowdzhq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxfjfrly.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rdbrmgwn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qllouzdf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2erujdbhu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bybgnbvn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mplsolki.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2czsdjqdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvcserw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zgjeqzqd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zetkgjpz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhhgqe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oqajslvr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oimzevlh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozmqagto.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yfkyelez.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2htujgura.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bzombsgo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oiaimnhw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pvrfgrxp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkxprp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2avsourha.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ewzeldlo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qeuigfqw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxsxuvmk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2peftalto.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lkcjfspw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2weoheusf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eefepghq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hcjbdtes.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kqukubsf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rzyrbivx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ojhtinuz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2azrlcvhy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2igxhtzst.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vupqrgqg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hsbcijeh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pvpktcvc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ohfnlizg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cyqcguva.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dwtsezjl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpxybsvf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wddtcgvc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zzcjgeqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sxaapboi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nwwbngyv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sgzzbnnc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gismfzaq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bnzcxhnj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hncabhnf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2muatdodd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2aeobhdhi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kkediakm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onynwtlz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hxputtgd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpqpjvbo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pwdupkxz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rgljqjtd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tjlmrgwd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lhcojlvc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dolurxms.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gmlubyqn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nmhrnggn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2skaaoyea.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2igqahvge.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2neoqjcab.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2chqugqgp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fussuawy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cpqucsnx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hcupbsbl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2godvfjjw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tcrtyrca.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vzplwfzh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ijhsvjob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nkntbhkt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2syrevdjg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lyhiyelk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cskyxzsy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wlnndnhp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xjtznrkv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2homkrlaa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gxbenozx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2otoesiww.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ssysuojf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nthasxns.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2abmvvqhk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sjqhakrc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2budysezd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lugaepdg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjgezgq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2goihfspg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dsqupvzb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xiwbcbwp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lwjatmlq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2pzhibdqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2taivhgbo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zgkbzafd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjxvdyd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ntchegbg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfimvy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjlwjmh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mfnmjefz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vqotnfja.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iapjqzlh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2deldtspf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2karczhnn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjszqpiy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2adkqrsqq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pyayvjdy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yjhctywq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kbytwkgs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlzwjgme.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gggzpviw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2egxoykvj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ssmblxii.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chdwgvyo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhqguypr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cffoxrda.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wpvzhwxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ttxmkfzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ghiwzldg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vtrvvqxs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jlvvlzga.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mpjfkfki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2sxegpzdc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eyrhiiwr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2usimlttm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fmkdmmrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ofncyvrp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpirhgnq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xembptbz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eacyxops.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yswdvhyo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2folopuqe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yuaindsd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvcrnbe.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2stzkbfkw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ilsdpdzr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yoopuufl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjqfvbwd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dmzfzilx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bypbcaxj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bhnqdbqk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wnuwctpw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tzydxohq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qvdovdwb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxbksmp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2awkncyay.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eilnkwiw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jhleskuq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wfgayrbd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hlafrsei.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hmylecve.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2houyscxi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oqzsyxjz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2emqgazdw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tspfkszt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2elyslvpk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aceqnefi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vsznrynx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mnbkothb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bdumhlzo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2brqeajuh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tdoektwp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yvriziyu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rpdfdeap.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tzqsofaj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2chvwdvtv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wmsmuiuc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qeswbpoq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qzymgbuz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ryittnlz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2aslqqcvz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dycatdmw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hvozjkzq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gqbwpqwr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcqllnf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ggtemqic.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2laryzkwv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rjutgyuh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ohyahubt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nlrzgsxe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ygpfqeum.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sahvovuh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eievvxcf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2heoxqeoo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2atnwexky.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dkjwoiry.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gobeiclo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ldanxmmh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dkxbniww.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jewyjpzn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wzzdpffc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihrhkbop.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qsnzzxlj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vjezxilq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kcslotca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hbjrmlpi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yijppthp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2yhiutobj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2apblwztu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kkujrmha.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkclbsb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2scqnsxqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tnlflqio.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lzgjjvam.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuasbbo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yiigldbn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cbakfuqi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dsroejyk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pbixlzyp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2masxctwv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ydkwoudi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kclwraqp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vtwckwab.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aaymvqtc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lqxvwcpk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jixrthuw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jfumwwjd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2elglglni.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jwozssqg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bmxgeahk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kpdqdwpu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jmslluuu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kgoieysu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rsulijan.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqhoxza.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwnkxkj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gftzlzou.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrsvpjf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2suertzss.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kdyrxthd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igmxunsx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fbpvipmn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhtlrfch.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ivuuvkwb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zisxokpd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aqrtcyfn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ileoznss.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bplirnbw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qaxdibqy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mcozlmih.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dyvvfzbp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2smymmtvq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfdksblm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zvodbesy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xqjoiqup.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqjjefc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sbtxcahe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2uewioraq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2idycieyg.html


<!-- 参考信息 -->