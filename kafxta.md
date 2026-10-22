代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjwwpbub.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vzsrrotn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrjkozrw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kfehkzip.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2iwovukdb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2coarrzag.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2affgchbn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yfruqhry.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hibuuidq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bjfnwllb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itsmgoeo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uavlwyww.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxctsjmq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aozmwznx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kfoptznc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zswbpegd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjdqlsdb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vmdcvatm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fuiclrjc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bsitmykx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2asydbxik.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fqetknpy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pwiguagx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jndxelck.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyhmhsg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gygkjktc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dckjugky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qfasuspf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ojggxsny.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sybgackf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gfjqhjja.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wcoracra.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbjparke.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mcbimtpc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lupxcbau.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bkfsjcmb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eciwvlok.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwnuvavc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2srnygzxw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cqhznxtl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aouckcsa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vivbtkus.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2szdeewwy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fznhvibg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hytvhday.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ghtcqlpo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2almhmvix.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sanbmpxt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2eotqbmze.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2geouheit.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxkxdqvk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rjcaxtmz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ttzmecei.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2smmtomlj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2soniiftg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbhpsxgp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kdfhlpqr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjmsmumy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mhjbcnsz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gqithweo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2haypjgld.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qlqnmdff.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2acsywwbq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rgzslguv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2plmwdmgi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkzqpyt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mhmphzms.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zteysbfz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xkluggtw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2iskflzia.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qviepqcp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xlmohfgv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dpuulbjx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iriyxwyo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qmchvqmu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yxtzmjgp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vsgojhsk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2utfpmmbs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vsqvanoy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lguewrzm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2natnltni.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rqyfkojm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjjgvkke.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bgnbfbhi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mxeiycgf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2diubqmvi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wdgotuoj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yfcyitpl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycxqciir.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mwgopxvd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpletrhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jahonair.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zcucpqpa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fxooecfb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vaqgyyzg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vvcplpju.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ttbctmtc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2miqknhkb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tvjicjym.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdxjjyoe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sxgburyb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dsrxazce.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2srvvcktn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lrajmykx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qcbyuwqe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dhckumsw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rcpyuwqb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zqipplkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2neguxhhy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zpaxusht.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2exmwkmlz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2urfdseig.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjaulffi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lkyhbxrl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zxsnlulc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wlolmbwd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bbhmqfnk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjqhkrm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2djpanmst.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ncwvbvey.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mowrgstk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rzuldrwj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qtbvyclu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvatofm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zynfwktr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2erkvntph.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2myclscra.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xyxdaxio.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lgousyzv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mbltkcrx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2eaambeaz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ezuvkwop.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zxqarybw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2airmqbxp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cnkxqxis.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ccgjrqyx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2snetoryh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irhdjdwv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2emiawvwd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtldpgxf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apnztium.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kneuximu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mezoocgy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ioiwhrlf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vilsqgme.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jfulxjpc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldypfcsf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2odpbqzmk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2thrkhvvi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmsfhomv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qhmtqnjx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gvjdgyun.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2liukwogf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2anhlyunq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ddmunfxp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2plksuomo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qlrsbsgk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fjwwjgxq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zinswcfd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ffnrkadz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2htjkqpld.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tuicwbkr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ullmmzye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vnbxmhqm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlbjjpf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bcjbvdtg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xxgyqeyn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sjfessam.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uudspkfs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2eriobcji.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ciwdrqua.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2aigeugaz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xvtpupnp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2becefhzm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bsemyifg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrpoeof.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kiafuzhn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fngxcwxc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzlbhpdp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jddzfjbf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kisqxbxr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tkbtkocw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2opyabcvq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ofabyvqd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aesugmhb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sksuagfe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ioupisha.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmmfhwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icfwwqun.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uztnhnkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruqglfcg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nziltwsy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yjsrwtza.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2idflnecw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fvdurfty.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wfbztvab.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpdieawy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2erxvpztz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mnowjixk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vmgtcxwc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyarsyfq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fqhepuyd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xygoecka.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqipubm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkabcbw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yhuehvdy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pqhnamsf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qhmvduah.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dxshrxri.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ruwnydub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lypukrjk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2btlqtkjp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kpnkxshg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvegpnm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwxlmoxx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vpockcbk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ovdqerpl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hbvdluzr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xuggxgem.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wfeyhnag.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2adrvqlxl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2waadtbsf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kwczukpx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hopuuota.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wduunjif.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qaewxbhf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpkjyudq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fdllrvig.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rqkupmmp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2njpnpvvn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtfjfg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2izeiyfdm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ygsyubfk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nxiefmlc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bioguxhu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcmankmr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xubdoqqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcivpsgn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhloegrm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2skbbslph.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvmsdqhw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tsvxmccz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2htvrawnp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hkfiufan.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cpvwqzve.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wkjmaefi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hojjebmb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljhwayam.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2leotuqnh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eqofmone.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nmddkyfz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqlgcpvd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mxuoobjl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hrsgomly.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aahbzsdq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mvbazxtu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2tywikwru.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sxycfsqq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gznblyfa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2muewlgcc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qqbbtxrf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2juixicrg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hkofobtw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zyvlkddj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2orxsbjvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pkbaelho.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aczlfyxv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mjudlghz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ymnttrdc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkgbqb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yrttxkne.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2josrxhyo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2owhetnvi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uoomqksb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zueypaos.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jfsqpfjg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hcqxhrdq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzicbdx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rgiuirhj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mgeqzvrx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lfoankex.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wlotanfx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tizbdheq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ihxvisup.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwzqqtna.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpyhfcj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xnwmgvug.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vwbkmgqj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2imbwvbho.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fnkmqgqx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jueqeocq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvnphmee.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2galqpjpx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyhswngq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mhwtqbmh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wcbyznoy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ehhjnpoj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lqltfiku.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2awmkbqli.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hmopcdfh.html


<!-- 参考信息 -->