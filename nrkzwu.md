代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqxsazia.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqydvpi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3exhqiatu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uzdqclte.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uxqbwjfo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tfdyqpaj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qwxjcwcm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pllhfcsf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3oigxqbgh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3egfvmvhm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3avqyzaem.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lqsxlqkn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oddttvlz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jpdkzyax.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hgdktcwm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sdfskygx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqsspqdn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fxcmjueq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3shphgppx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdazjde.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdwqaku.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mqoqbgte.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kaxhozqd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vtolgnrk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hpacnyxt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtrtgdzt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sqpvxqfi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3begycvbk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ggounmgv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3spxynktz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3htxmmkit.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yozvicug.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylrlpgce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3guxbwjbo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jolmqorj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vpowwxpe.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kldbunih.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cmrkwfge.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cibjwcbl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fmecvubv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3sfmjduzj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ozljnwxd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vedwuuaw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdzvsvyv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xfjhdoih.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3landqosf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ynxorgbp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rmblhkxi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hcmyksow.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3oybctkoc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3levbyfpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dkiggwuu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3juqubdbz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3trdatiqq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kftlkobi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zymaemis.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3uqjlgfcu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3puiqnxun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3itbfsgfh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bvflpzpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qwkdnicb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wrxeetoc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svlzghha.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3puccakmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fghcmamd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3djzdwzrp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqdlbxo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sugwzbwu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tgmeteyq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uarzlmgj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqlemizo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3upuhpmld.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mbxnauqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hliakolh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xerpduhx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3idykrvvg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bilsjhci.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3iovyjqbt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxrlcfud.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbiqbngs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3itmnbzju.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jkqjdepk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lwoyiiti.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nqpramcc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3abrdrrmy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lzfxxqzt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tdsmffxc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmofhjth.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qoehedwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxnmnwu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxmymgrv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uniaocxs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3telgibcv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3phntxdbj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrcaolm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3khmzhrlr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gnekzyyf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gciqjclu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfioyrl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lfpyopid.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xrpeymop.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ncdbqzuv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ctmtvlne.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oypbzjms.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oudrpgtk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtagdvf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3trzesaxa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3aakmtffz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cgfqiwyb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3snnrygki.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3aauvolkd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lobxpmnv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vasnjmme.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hvpozoae.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxteyjzg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzccczao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zxutirag.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3goxscskc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yqcluimd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qvczvtli.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kyojknri.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pkxwwmww.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hbknfcxe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qloczjnn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3meaxhklr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ibpeqedq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sspppija.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdomxfdy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmekrwuc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cmtvgzzr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arlsfnie.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gqjpiibv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrhfabqo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nofqjdmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3scphowpk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qwdzccsm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fkpohkik.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nyitksjl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3iildvscq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3skggqbvc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3srooxvfx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3szaghjhw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bepmoetq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyrhnbr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkwomafg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzujwov.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yijgyift.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tacplixr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lgqnsajs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ldtlhkvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vnmpqlzm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ubavnyxf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxhcwxj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lyvdvacs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3beezyiyt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qrtvjoiv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ccnucjrn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3utxmdrjo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3caplinrf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ctgrnnjk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ohjenkcm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eyqkbwsb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jnvubbce.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsorjhmb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rhdpgphf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mgicdgxb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjwvzmv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3btgslwph.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3icmfjlce.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqhcvjr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ewkembfl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jkmkhsto.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pbauoppk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wqqlfuby.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hsyyawxb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3stomfhjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lspswyfp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vcedunur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbzzlpjn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3udrjhkcq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zteaepam.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajghferf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bbvibcrr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3goecgtbu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3loqxymlj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3scjbljbp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3urgcoopq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzguyufl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apiekctq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jjuakjgh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3cokjlkbv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3emnhiyfb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wddxnoxb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yoanxvnx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uezuwwjj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hjcyxxjq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zyufpnmp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3krgeewbe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vcntevmm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uzhbohlo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yqucysyg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uynhmfea.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wqsicmuv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zcchengv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gbylonur.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dvzpxfyd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lbylmfsf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zztfzifs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kusrmeqi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jscxkcpx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gbvvzoma.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uylgwjck.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3dztgjubv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzgahar.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uqsqerad.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hefccwrz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tyewuswu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3omokjfku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zosaxfjd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dsiqtmme.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bjzhhmte.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sofdatqo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3htgstqhm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ffzzdnik.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hwgzufht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yksdcxwk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qmeycqse.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krsqluig.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yaeukomk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmpuqubv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnzvioi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3himboybu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tfffmcsr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gotvrurn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fuvommkg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wbcutdqd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3koeoernd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wqurraxl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zwdxzlch.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lvzkcrvv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nbkttwhf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lwpgcddx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ltxcovne.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ctokdqqv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wbjelubq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhayidal.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jkwahkvt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ztzohypf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mpmcflvu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hbszpykn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mcvwaeol.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fnkgvxbo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmqkcer.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btejlelm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aqakjbfy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwhezjoy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rmmhlyuj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tlckutgy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rujzbrnv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pcqgxrpd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yvewtjgx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bfzsdynh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rgmycbtd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yrqszspe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bbwcwrgc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cxjxmncr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ypubwrse.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ficdinfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rgdtdmvb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdgffxqo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bxkahnba.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdamextv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yuaccxwu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3izroslel.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3htforqed.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wugaljqv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3atwwedoo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ttnijxst.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aipkqvak.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xoyvjtqr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tikyysfs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cvrxjsfb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mbeonezx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dcaxtdnn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ijckhach.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jlgeszre.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3svdojpmi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3sjgpgdxx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gtwrbsig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsjnghy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3duyirkji.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktquoick.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ssoeglhg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ltcduatk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oysiwpcj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilaufggz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mvqbjpjt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oasnvril.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3puvcwyrp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xjubtkzf.html


<!-- 参考信息 -->