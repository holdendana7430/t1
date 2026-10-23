代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ovowalip.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmhawmmh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zpgbmyah.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ubplifml.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hwtvviqg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ogbzbtrp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnokzdi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uazjsxsr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wrcarbpb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qkegnxfl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zuootgzd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnyypjxi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dagkbywz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hbnoczuo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3otzzkaeo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zttmthkw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bihplsrw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fczwjalo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qiadpjgt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vfrdazve.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjzuueo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vklxaksb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ujlqlxbj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ccongidx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rclvigrv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bphymqcy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xeasfjaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kyqwoxbg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gtrcdkkl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tqdopvwa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3amtfleab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kvnevree.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qwrwpuzw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ylhxvkqt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yoirqhne.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wxljoppk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3izfzaoji.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jmrktuhd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nibgxauk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3guziqwaa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ezhjlzdq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3taanbpte.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wffgyjkw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3suvybsen.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3owoqbjan.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rlvibncb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jiceeevq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zalawfbx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qisftqxc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dvcpfrlf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3skahknsg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fdzwshsh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fivnkdmd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3swukzqoq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxsneqli.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqypcmcp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xarmaoey.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dryqykoz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dojepjkc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qywfjwih.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jcehqxqz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3miizswwf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wjypxljz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmdluprn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cgholzbt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hevmzdjv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kgukgzzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tygsudfw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3sglezhdc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lymdralj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yvvuzgrv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qpavpdcf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mfcffcni.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rkjimqmn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qgqvtyqz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fsdwplfj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fwqtalpr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3djxwpxeu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpofenhe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jcoattwb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vxsxllpu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qozpflzq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3agnrwwlp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3sxabwzqr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ncxvvymp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3acdbwbmn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3blvnyrev.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlpbzvyq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ysflisdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3inliktli.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srudvowt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bidhgcuv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcscitz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3sucxcuxj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3abukrrne.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sgqllqer.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bsolqxhf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mxzubfrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rnowfvbx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mdergmti.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxxbgedj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vbutaquz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ldpdfoky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dobfgwoc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fcaneguh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dntmbzlt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3upqrcvjk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3cmvlmfja.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nnchqhap.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hfklybtw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3okkyjsyo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrsjeei.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jacwctme.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kuapchlw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwsypkyo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amfpreyg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cqsleaqy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tqyopeev.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ooaiuazf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pmlnmqfq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3btizcfwe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dulmudxj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3onhboevb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aevbnhrx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ikerbgwd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rpbbidaz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvdmrdz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lurtmxvj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3srhcjkvj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlkxelq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3puskbnms.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rquwruuy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ruipbbes.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jyranufi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnjetey.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rnexrgus.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jnnligdg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bgzahhng.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mqzcjkzy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yowgcnev.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mcljrfeg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ljzmqgdn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xycwvevi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3inusyvlh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqesolas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tsdauush.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dxzufuda.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bfsbssrp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ybuyznmn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hvbdhssd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ojmywesk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rbigvcxr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rawykcle.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zepbuxmy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zeqtjbrz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgpkwcf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xczhxbkc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ddjnbysg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lriqepyl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxsagxz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rrqorosr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yiuhaitz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3raxumdxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcucihpq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rrzakzzq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3majzxsyk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zflbrfhs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qpemsihu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lxcitdov.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3koqkabpl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3emkpnoni.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bsxjpkwz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dfvlajpn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ctsfstdf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3chmmicnt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ditamypv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyuilglh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3svjgtitq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkujamqv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmtgcypz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ywjrsevd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3djbuijvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jhzsrcsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yasfilnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hiyxxbtg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hpwatsry.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ghkernsx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rhiupmli.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oqmryqxx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tzwktvcd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dpcyolkp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whoyxllg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3baznckwk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfccqaab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3isamaymz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzltsz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hkrcfzye.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fkdlnolt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpnfew.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zzdspjvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hntwpagw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3egcfocrm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rfioaomy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lhvazvox.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zjvdnqfm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxgfzdu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mxbrljqi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xzwutxqq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kbkrobic.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vijlimuo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3agnsyzde.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnhkkisj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3eauwbhym.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yiotcjfo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqztpdns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3iqlwrjil.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ptigkkok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wmttchhm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3popcabmy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3efqrqhpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uewoflgi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nkpupuen.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3klatwrom.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qcbcahgp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dbxrywps.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzkshei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckjauubo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjvikorn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivgsoskr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zxixqfrp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ltvescor.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hqkshhtm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ikrqocxj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3brxtxymh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cjwtpled.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nayooccd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnowrrl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xteajzek.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3brightze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvxytjed.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3veluvklj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3egptzzov.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rafdypqc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vvyifens.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3edcuagab.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rjyuesct.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ctmoowls.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jvcfxths.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kxxcedhj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3blmppbkl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dfmhkvll.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tqbnmnyx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3taydtjto.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3morneoyb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qzgokuin.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3alhhjqmh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ukcrwpds.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3acqjmkwa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzxhrnnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rprlmcmk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sywgrglb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqdytdef.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gpzevkum.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3btqhkvcp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zrsmqxuw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vjozpleh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrtgxwd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dvpilugm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3semozqjt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iizgowmh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ecjilnca.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nvcyogwz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3unyqkxsw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zoyoefri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qmqusqbf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hxayvwek.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xvsdojes.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ihbqbnfo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iyoaymmf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uegufgvb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vifgogbj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wnzgfvcm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qpbvflnz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3iomvikrf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qoikswlg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tbtntfiu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rrlpipkp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3crepival.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jxnyloyj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kujiuumj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggltivwl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxwvspnh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzufvmdz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pruasfnp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3egdximkv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xjlvnmfk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rnawdnfi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wvihdupg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihvkahtd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lfowahjz.html


<!-- 参考信息 -->