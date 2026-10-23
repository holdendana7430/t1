代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbpbdr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hfeebtav.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kitwbtny.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ycinobwf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wodlwwra.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3muotzmoh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bxnekjym.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3eybtteiu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3iwankfme.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uupsakzt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3siipjmtj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ftqfeuhn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuisruab.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3giakuwng.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pjmowqim.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwcdof.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vuokkbpk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wskruwej.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtxcwafu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bwnkwvcv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zeiyqtvb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gsjwzpxm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxxvyiea.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ckbvecxv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eqpwpraz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vuvdsjyb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bzkozyky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dghdhivy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yiagnlxw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3onhbwugj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vwziaeta.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qqypueop.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxttaibs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gdsqjhwk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zsnueyke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjfefeq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nswcudfv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3grdohque.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3angteigd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3etmmjyzu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zmqshrau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3znrrnvyb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mulqvqoj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pnwszrqe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3emgankxz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hjuqxvgc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3conyktiv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lepbpgyo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yvlemldm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3drxurxoq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lczmtjco.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xvvqfrfq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ilxbddmy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3texnbubu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3usrbcspp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewjlmrrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfkbvjj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3afyzpctx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xihristj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3daluirrm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dbhdajaf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3egxjgoyh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uqfcoxws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrnyie.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hgbfhttg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yebkluhx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zeubovov.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fksxhcph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tfkcabuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlhgxth.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jndfpiqh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ccvfaadh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3grhnzmjc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pzuvnfdc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkulctu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbmhdom.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nvnrzgmz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wemqxogv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhwsjgmj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3svczmuva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ochdcnmw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpbtueyk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwysernc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tphvuvjl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vfiviamf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gptkdnqc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mtxqoxvg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3loctmdtk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxojdhkr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fqcuvmla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcxutmat.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrugldlo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtzenyes.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lghwgsmn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xvtyulpy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ersfzgrn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vtjtocdv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uzhsrjnz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xnikfkll.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilpzypnp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwocylo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3weqzgjpb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcgrwh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3whfmmsnu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxblwtfy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rheczdos.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gbacmmkd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ddkkxbag.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wkkrnhvd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzxifsx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dfgaloja.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rqqprmnr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkoycyra.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3otmlmmqa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mlbhwdju.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3htdagemz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghkmcltr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdrnbqyu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gjsrjnzh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wazliyyx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wetzcxfv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zzevtrwe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3oimumxtq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gveaqxht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3igttoeie.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3cguhdaeq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xiyukubr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qonrdvph.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3thbtklyi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vkzgdsjr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fzxbhnna.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3laosauth.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cjgygtjf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3plmlcrxk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ihkqgabn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qvzholia.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rhjkliuz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cnftezwl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zvrliafl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ycsvfpzn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qkawqofm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cosbenpf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxfaigh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rsqooeih.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxfchzku.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ezfkoxds.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xfguedpa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dowalish.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dkujclfc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3phkpehzs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pubfdgnc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dgrvhuav.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tltougtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3toarakrt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3autozhay.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3agamtfgr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3malyejxz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3sftsdwbt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3obypaecb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nsdpeqxw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuczprak.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lblxbrzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bslvlojf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3egsbnxdz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3beelifpr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmqljcuw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjpiqam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqotrxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yzuyboeq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lffmmocq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uyqwlwcv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nqzotlrr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nhduvwah.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lgzmnvzt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ztkutlwr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aaovthvg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ikwggrau.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xhduvfhq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yzxiykbs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qfqikxyd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ztkqfgbs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmevluhn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3degghlrj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lvzmjtyr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzszygg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zqvxhmpf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3frucigmp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3grwfxobn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tttbiisz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gkmhwmxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyhdpwue.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tygbojpv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uivsjfpo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zlckhbpf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ccmthqmx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ixsqfrjy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xlwknrie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3houncebe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zxsaxkzq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ulwteyuz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gbvkyfyk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cfrbrylj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3szffvfaj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eaangrgj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqghlgdp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqppzci.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsurrsj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iaxuvaxi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mgzfgwmi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ipbfqjgh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgcsqqdy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3prncohht.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kycqjrrv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ttgjqdgz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3utexsgpa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dmiyeiex.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3djqpdzbl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3udvrnqkj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ldaiyjnb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfacqqes.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mkefdvig.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fgysnkbj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xgsqsbil.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uyvmezlm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yvhfmlac.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdatgzrk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pamjjzhi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jpotyjkf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ofqsfnaq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3spsxwphd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bylqqeke.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lvosdetj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sbzehlzp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pyedwfar.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zmcqxvyf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zmdmvjgg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pwdbclmh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fbgegwvk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsanhuvj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxlhqwvt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftzpszhh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmyrlscb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdpcqlm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtkitpiu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fssrydci.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bnryxvzx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lykjtmoq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rgghtwxd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3guqtuaov.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yiqscvbq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rlpvkyus.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yarpxvvo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xgtqzltt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqyvgvp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3zmogdmha.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zlaqnuki.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jshfkakl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dafpjral.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kctcfqbk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ynwwrjvm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ycbprhte.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vujsryuk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcpqavs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3oovywpih.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzderkvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3azfciufy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ufaduliv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yvlmppvf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wpjuxuvu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nbevmwyw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qcstkzuf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tyhzkcec.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fbcilysc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3meyxmxkf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sinvsskx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3elnstsvw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mucosdvm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bzlbergh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qvaylshg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lhscufxg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hwdvqdri.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ubtyvnjh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wnqrovve.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mrvexybx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qwtihugi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gvrkjnqc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uslywowp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dzwrpygq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xnilxbjr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ovemruwv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3uabiaplu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iillwwub.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3iizvbnhk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vayplrve.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3njbvjnvs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3agsvcezg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cbfxxpxm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ahpsmcsd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zjqkzsay.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wlaibwsn.html


<!-- 参考信息 -->