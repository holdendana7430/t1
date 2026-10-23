代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ydszzjtp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xwcowhsm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bomkjltl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmvdut.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wpyvznoo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwhjkftd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfdxozda.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sogbtfdf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ybxafpxm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ykvscgoo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tqsbsgod.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3anjvsxrn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3uybpqzar.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vegekueb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3swodhgws.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3csvixvzs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nijflzux.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qejzxkgr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ymcwkxzn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ebteqgsl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iucqshle.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hndfmsfr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwgmssvj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jyqypdxg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vnmwjxfz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fmohckoi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mjswhiex.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3anngzwew.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgwxipnq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nclyevak.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dcjbvzqu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ovhqzqiv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwtdsdjx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ysoopuai.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tkcigycj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hvrpique.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjextiok.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jjzdxuhg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3utuvcfto.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mpspuveo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iimwfkaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dgtqrfek.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zisipohz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wozywqem.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kugtpcfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mxmdndhc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zfycjrfo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3safdevni.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gvoxaujh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ybppekgu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qutpsrqt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ymwxkgvl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wlauqdrx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3guyespyj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ihooejci.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ytnfyptp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fvrmgogu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wutvefru.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3seorrtho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iamvgbmf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ifxddwvs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvmxofq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jhigqygg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aitxpdai.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kylhvmof.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xdghoomo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yastybpj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jasincis.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hxjqppaa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxljsjf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqklurei.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vogkempm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tpjxttvs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cwjgwvzy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zzlfctkp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vmyuaoaa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vxixeiyy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hjrsawpr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbxaiufe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3opptvvsg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pxrulhob.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bzftgnnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dizgwzle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmwmuegf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wboxxtuy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bnfhvujs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gozcpyia.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ffdgkowx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gfcjixqc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jtbraylf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3aazodolh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3trgjeymd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dscrnipv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3glmqqoio.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzvzclvr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mfrcynqt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hhlahesp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nanhbawe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rdddoxub.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3twmcmhmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jmlusazw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nhgeipul.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqgozsio.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qidwkjno.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkzouoml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnxhprn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3afmhwqkc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hjarocni.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3abgoeqqc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uvpcrfou.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jsdenbes.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ptkwmypq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xokkacsl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rzpebgai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjqaqmy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3btzardwg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywxcjolo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jzuhjkhl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cknrxdlg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bokqbrfy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cfdhemrn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oteunqbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3azsaeqni.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dxcjdhts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3olpyxkoo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3krrmtaqr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3obdbuleg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hinxpnxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mqrdoikw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3oqyuryca.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vujucvvj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqzvpbvr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nlthiuhh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nbhpfuvs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gznfqbih.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gitsflox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tmhgftip.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kwegmzwf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jukzwkas.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sysotchq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3evmrxerh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvvvpav.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xztcgxgl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kawdukye.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aocnxmze.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ulcpuklu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvazorat.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tinuawxi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvghqsfk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yoegmvih.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjhjjztz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dkgbyqmd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qftvjwvh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ydnqyjyn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bwcwlbmd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3utimpqiw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3upkwuflf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tpqudgok.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3redkrqnr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3izgjowuy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlfebflv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3adqxqext.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwpmuktp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pvmzgqos.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3isiedpjh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pxbuigxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pfenrabf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vosqbxvv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nhbxnout.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lkrylgln.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pquvfrgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ekjtgzts.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jfdtqiko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nfdrlaks.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kpwqpgei.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qobzzixs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ahyclsxf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xcwzopuf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3llfernqb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfltzird.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rfpmjqce.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ostlztfu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3udmbgyzw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kvtbpits.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3afvhwzme.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yruwuykx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bbwlcfct.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3seznvcyf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bdfolddl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hqccomyl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jkbrxujj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhbtujx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nahoepiq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uafcwhhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyggbxrk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vvrvxcwi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3gexohjwt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oheducar.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqpjzqgd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gvrbwqvg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3thjupwhg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3clpjgbxr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iybzcqwk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jseiwogg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ayolyenn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yfdzrzlp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3onkmpjkd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwgbjan.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3utlziqau.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ojtayuuy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uyudozkv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gvkezqil.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aiihnqmc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ooiftikg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jscgktxt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ydkdjtje.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zrobdfxo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fywdibkv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zsfypvop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3djrrgweh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ehfylyrf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3herkilsx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jydrqxmx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nvgizxfw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3meidarkc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nbvtjznp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kodjqoap.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lejziksa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lkbgfbdi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3phtskfbs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tiuykwtv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pjutdaxu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qglxxnkd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3apzcxifc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3etrguwxu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zffsblgf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vxfuizzc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tuxzpseg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ocgvjwzt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3djmupwon.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hjwbxxhm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hsigessg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibwggoxz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhawyqc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3njgugtes.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kyoyhelm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qttzqlym.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxexazqn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbtxpild.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rlneurxz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3uawlkaii.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnphsfaf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zwjyckti.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ltjtdyeq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3weufmjxm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rxejiahm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3skpizwbb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tgaoanhu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wspwkwdn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nwpbuzjw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hebrvxlv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3raksqfrr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yrbziast.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3njhgdmeo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xqnkhklg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hazbrbyu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lkyiuqmx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vsoonstv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3putcxmem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lxqxjtsl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qizjwsxl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3avzkmuec.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3atjjpaze.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxarbfkp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zkezzivf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sipdocdz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ewrpxsfo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzsxvys.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xofruiev.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3awcjybee.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nthibakv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mfltjexm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wevozwta.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3slvextgx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jqmhvzxv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uqguhxrv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mhmvgwxe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mkkejzux.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hurccszj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwpdxu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tavegpsp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3skzsugmm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3khzrghdg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3flhdgvyv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3inuqooue.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3deaigvxf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dhxrsxmh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfqzqlzb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsmzbxgz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zyhfftqa.html


<!-- 参考信息 -->