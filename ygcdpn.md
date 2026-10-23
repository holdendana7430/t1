代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zhsqgrzu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tqarrqnn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3npkrbbpp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zkmgxtcf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hvioxizb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rhqzantw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmclmu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uqnkvyuo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yvkyoigv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bftgytxk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vdrkrgzi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fnnmsjsp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wirgsybd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgwzsvbx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ivfhrkya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mwddprkd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kwqzvfqx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3udtchmde.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3meslihjo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqgmcsb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yjewyrrm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3corioulw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3quhgsvrt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ruclblsx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cpupfiqd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uilejmbg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gzowahkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vimoszgm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3htpgtkeu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gfucbkhm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3pabwgxly.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jslgxhim.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xqjljtec.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pyerufis.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xuybeqdz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3sihxjkwv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mpklxbcf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eqcbsyvv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dinqnjfh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ytkzusax.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3oovuhzcu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dwevjtfv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3idfqginc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbacecn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ugqpymuh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3miqmrcxp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wgylbpbl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3klogaqfp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcxkyxv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3umyejzum.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cpwxnrgy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3swtqncpe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahedvmvb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zmyolcrz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gdninlyv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kguewptz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ksmqbkac.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3znppqmqv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaqzyggv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pvkdxhxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nhypoaqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3alcjopgo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwlfdgs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcyqubgt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bwuknjwo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ulsrhtqh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oookbqhw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfjhknes.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kyacfiqr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eneogrwl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppvyfhwh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3syfmejoy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dyzbtpfx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ssuuyprr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uwbfbyxo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uzcqdkcx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3owgkiyio.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kryvdsvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxphqois.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ueooucdz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ilwgewuo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjbtijj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kijjmyhn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rhxabvdc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fkdtsbfb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3renvliqn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sjprhqgk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngskufhe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrcghhkr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zflvzalr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bqjlhwpa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pgahfank.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpvvmbye.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3prumdxym.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3agmylpkm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bcpgdvca.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wvbkpgqc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3stdbmiby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cddefeam.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3aeespyab.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wqvqoqix.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijvwxzlm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dzvtjarv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktqrnoho.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mkhcqjlg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypicudpc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hdsirxds.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rjupnbqi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3coxapipw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ekhdango.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bzkdgxjv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bgveyyyy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3eloywjnl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xyfbtmnb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhqxcxih.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpezkcta.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kfxhwdlb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fgrxtsdr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aeqopfmy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hvcdujdm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fabdltal.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3eimzqway.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mavupbpt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kgwuthsy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ccctllae.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnqmqmi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jchfjtlr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qvvddqey.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svbzbsgz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlmessz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yyuwvnrx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ltrtaqlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eolgfieo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3enhxxwmc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3idridqlj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3afktjvlw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3enfesiby.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cldaffnx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fakbmfdd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pdvzsszw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3miahlccx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vzxuyfwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frbtixls.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwtnftab.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iydbfpqq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ukgbhfez.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvxomxnt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qyedhkmd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3szgvcaxj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zvkjrbsb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bfezxiup.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nljggtsh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jimurjqf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzpcfyam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3edaaatqb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rmeghnyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rgygmmbg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kyxfxxys.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wnbrqouk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gdijrajg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lubnbklu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owjlzzyw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rymmufhb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inyrwtur.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lfnkzcnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjausftb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gmzmebjk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wvbazafe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wgcgwdcr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhbjiqmp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bwjtdvww.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aoflqdyo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nhjjshrn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ndelhoon.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzijlys.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzfcgjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbmequjm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qkbosbpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skmgzfga.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwzvcozw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qenkgpyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzcbrdkj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lnuqlgxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjwfsx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bbfjadag.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqyppywi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uoeqnjev.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wgqlsesd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3htubazij.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mkwebkxo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vukjpbnj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yxjrehbp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3luodxhrv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qnnltgfi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cpmknslo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bbasekpa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wunochdw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mcumuexs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gbqmryvr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yjxvtwzm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqytox.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3veqbofmm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bsesmkcp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aewhqqyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tubpuigd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ovunbsbw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3whtcqpao.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gyoejlhd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rongimjo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzibvij.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pysjzhlu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iaxvdchs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hlhsevhq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3entceilv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wlorvaqd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kqhedqmo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iqiazgsh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xtsqbjlq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3akxnjqie.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uitvgits.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ckighrlh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zgaemcew.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yhnqayen.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hntcxofm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kinggqeg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3keahrtnu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvfmvrhq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3arwywdvk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rwkyklbc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ggjgqhjr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcepfncq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3outwrpzp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hfqwdorq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xttszcvs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qbqqhkop.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfmzhfwx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eakgiyhj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ubkjyyvq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3uzjzsviy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rqagapty.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3funjbdzy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ponewmlv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vismszhv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wtezqisi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3udkkxfne.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fxnhvqgj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3powirsjd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tjsdaxlu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hqazvakz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iatabnlc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vwcyfuie.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kzqddsvt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkdkylf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xiooempp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ddwlrcxx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cebitfaq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lxlhwjjv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zyezutrq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhqyste.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hcmytsfo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tzyxkswh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3datpbixg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qutrssuj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zuzuoqix.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prldrbxc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nnckmemk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzztcyl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3avswyfbs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qcoilxiz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqbqgkyn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pidaaonn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jidkhhok.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fsdouvid.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cezmnzzr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bvrwiidw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ibdqnait.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hazgwgeo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fhztytdi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ckaiuejt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3frymmdbl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nvwbcucv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkdocvly.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xknbxdep.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pdawwsin.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pepkssog.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yqyhyvri.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vjyapqie.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxysduyo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hkhcarjf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3owjcwjef.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnjcjas.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spaumbzd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3okypsskk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ifoejjuw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvetcf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzikqojy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pdbxawpp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pabxmnrq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3duhzomen.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oltromdf.html


<!-- 参考信息 -->