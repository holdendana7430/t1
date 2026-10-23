代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dxktvrpn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jmeacvcc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mfozjija.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qcjotlkq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hizqbhnb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cucmvfxu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3civembso.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tardizha.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bjhdcmuw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmansqdf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vtpwzzwy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3iemhzytb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tscqhbtl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uzuxqmnz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uzwujrsb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgwwhmks.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zcwnsyyb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ublgukaa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qgaxubrv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vwkjiuph.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aqiwrkth.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pshvyhao.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hokwoafj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qgearlsg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rlgzfjpq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hayrnqnr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iamtjetp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oosdvinl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfvxibav.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xsybxgpn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xthqastm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hxklhdze.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fotvkqep.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3givbkjmg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3sudqgbrv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lsjzlirt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmxlawid.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ghlshxap.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pfutkcge.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sqzpkghs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ztivctdu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwtsunsd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bapzxjud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3idtytopy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yachmcbk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dyljaznb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jhsnzhbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xjdqpyzy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3janufpwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dtumpijd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fphhgwgj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3sjemzjzm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nxilfvoj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3frdzkyvh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oosbzjoi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3giyvidmz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wrakbcyp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fgaedaay.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uotxpbzi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dutujrfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ksgryvsl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jzmdmabc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3aevfruuq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3giacqxvy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wjkipyne.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pqbojadh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3duvpbvtp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vrfafioh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3njvzlsuk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sgsetunu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3llozwtyw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zxedjoov.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3liesrtth.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nsygkdct.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gshoznhn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hpscwxfm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxwynwfy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pvntzqer.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3avmfbjdr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gckkmxqv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qdlzycmm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aqcmcpeh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xotfvstx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecfhnkab.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ehyeseiw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uxlwcdoe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3klrgbspz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rkgtvbyd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nemtgfgf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vuehhduz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pldljioi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3njqdjigl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kqkfuctv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3plhogbzh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqyymcey.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ushtzjvf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jflcrdpl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eathpogx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ehwszjhw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fzghfurw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ogpslsvy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3etersgis.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ttfljypg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtzysstf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmjfygwt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dikpbvtc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ewvrwpuk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ixftyqex.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynmwlwlq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xozbjtmq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3prjkdprz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mihzionq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wbujolst.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xdohlpid.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mjuohvwt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jupmmjfh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3phllrjzu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tcxggdke.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qcbwshvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xoqvobjs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3usklvxbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bcwhfrjw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oggqlraq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hjsettzv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3miqruijo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lmtqvdgc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3glvpuvla.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ihtnzmnx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rnectetc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ruwmyciy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnoqhmx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqcasamp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oqavpvfk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cffvdnzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qkyucjfl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vfronzhe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qetetpuq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qrlgkbuz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fferhncg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xljcokqx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3egkliqyk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fdudihtz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ztocuntf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdfpzes.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hlaqevon.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3anydhxay.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vhpczlvg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3edaqbmls.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofshycga.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pmjebpfy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmijlzke.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ekwuaysl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tsmmpidh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3icqlznej.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yctaukmi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xgldwkcr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lepqebpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3otgcqjxl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnebbmz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ywygtqfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxybntvw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3unycsyiy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3peadnjpa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kvrvcwmq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3okbkylvs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uaetauoq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fdroqaxs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nxolldgb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjoyczdu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vswoakrx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xdlcbkzz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wfvhwxqx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dercznyo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3olpfyohw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mmmddjpk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3srltpnpi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yqxawpcb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jtsmpnml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hqnuniwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uqufdzzh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ffsdzkhu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pljlomvh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pnqsazdu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvdchcct.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3biultyjf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qngaqwlo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yfepdorn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bwygecto.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hjqrbmdg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ivwrieue.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hvtfrpmz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cqabustg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgcggzbo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ozoykfqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpoekntu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rpmtphnt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rqxsbdel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3useutkfj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ywhhibgo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jkkucsrc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jbolblgu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ppfkhney.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zvnqhmew.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqggkmb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hjeisttw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pageboav.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pewbljxm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3flxukisl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xxrviolu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3snlnbelz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtsdhyx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fyqwydux.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sbzkcmgy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pxrejrea.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ymoqvdgk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nikzdjyi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ldcijljh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3asiprwxr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzodngi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bctjgilg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nldxrftz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nznootjz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gvfywgjs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cwihoorw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fctqsaoy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbeuxgv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fxdhquwg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3owswtxbh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3typcztli.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wmzfzqfx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wmgjcyhe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3moxrhjoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gmgafkui.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3umvosnly.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3shuuimik.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3afwtvsoq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rjindzdg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3afsttnpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3injogkto.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hfgsbffg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qbsyjcgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xufqkabt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lhvdrqsn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xyxbdagu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bsbnwleo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jvbjcdrm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmmvgru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fcelakjv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cqawjfwl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ehypynfs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rjhmufjz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zharrorz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wnzhqycn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qpmaspgf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3znaopbwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcppmvyh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qxqguukt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3njqhcfhz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kphquoya.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qrawvryp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ioqfcrhc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nwqgczsc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3whlhtnet.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rfopzduz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3oofewtvz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xbxdgxkq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrlhnij.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kxvygyeq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mzjycdwv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wffwdpsf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ololvttf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3slputzyq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kypjolqo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3exontyoj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iudkibka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ipoaszct.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jdoxnfzm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vcprlzoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxwjsx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ueubllnz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wgdjomsu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vbxkmati.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3knzytfjp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gmutvznj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3iewyetjx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bdxmwise.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vxakcusc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zsyiqntp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3slnztzod.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3leydiynp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cfxbkxcl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mvizyxjz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3youmfgmy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wzvjvgnv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iucpoqga.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iqaoepkn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jhjudcxh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jjzmirdx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3efsovsbr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sbzciqny.html


<!-- 参考信息 -->