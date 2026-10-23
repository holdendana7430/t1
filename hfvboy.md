代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ulyjagbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zauwblvl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dxvgfzbb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3txukswzw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoezlqvo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xyzjkkcq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cugdleag.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tuclqpsw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dmedvvns.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnvzevqw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eeynoghq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pogfvlsr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xjcafuse.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3suneelsl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tyknkddn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgenplxo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3varfmpum.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kojmrwgo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ggqxeuta.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vwhnecwh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cghahqqg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3phctllbd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ypedkxfo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rcexiouc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hxearuhv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qtejdpyl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ctaguddt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xdqvwbwm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dqgzqwgi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uyjqiplt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ogpjwnja.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ztbxmlzz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqodnjj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yjkxeozw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qsewslwh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lotzkmln.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sewhzout.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3utzveoqm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3epgedrgw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3oavfubuu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzbaqvk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lnlsxsvo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gpaqgaij.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ylsguxmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nvldjixk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ahrciyur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xeknbyle.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3afzrcgan.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cdvqcvma.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ldmvgxrm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vtndlcyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lalehbny.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vujpxoth.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jyzbkifx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcrmxvgk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cvbpkbtq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qwbdnhyx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3omvdubbw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vyusjxwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3aajlolto.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jzqpeodl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aizwvstu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kexmtbza.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uorsyfxf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpcuydzo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tavxrrdv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fgvfkjyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ofspzrfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yqyvtrsw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdyznqer.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrugjkqn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3endxotvz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3huzbrfzf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3damuqdir.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fybumniw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qciplxpc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xjcmqriq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsluojpr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3luzzybcn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hvdyrrdx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nbrvfxqf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nriyvegt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qjpqjjct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wxrkfipv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jamjvvwz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xgzrgmlz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wpogdmul.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3huyxvoss.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kcdaruwk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nbnouqyz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vqlyiixc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tpoukdus.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ezjgwlqy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nifoojxr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3omcbhlxc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqcuvpxx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztulnwqa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3voomfgge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ykylvyiv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kpxhlbum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eezxnavg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jvxibiyw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cktnjjeq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqbosew.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xmzbbpuu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjunnmfq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ovxmqhxp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ilfmfqlm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ooejhgph.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kvgvflgg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3epedmpva.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vzmfpeuh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zcmghmaz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3eiwqfjtz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kktkyupa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tulzvuup.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3icupvthn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wkfdkpme.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqtkwo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pvtdwiow.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qpveglsc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdsvjxbn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vlwwjwbd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rltyyura.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3quzpcuml.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pqeprdqw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qiseysri.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3llhazelt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fxcpkubm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kntyiiyx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eamaewxc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sspuovwj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vbvuogpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tjewcvii.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bmgfojig.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ecypzffs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3clamespc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3owwgvlgi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pwgghncm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3erggmluj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dhcbeoxy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uacckzfj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvsfsuox.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzbwjxl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcgyisqy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmjixzn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3alwuaefv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3utvdejmh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsrppjrp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hfimwkye.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nftjewyd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ydfyirhe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dtukbbxs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zeljkwdh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3amrzkldc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3otlsnlbf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3orzfbovb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhcrnkl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xzxtcrfz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cjllrujt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qfyzrhqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xytwwrjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mzhbwdux.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fdeaclyy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wezehqeu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vcaibotp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oodjtntj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uwfchudp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lthyfcjs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3snftoqnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rdsggfli.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rliwcyhx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mvqqwqga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ommihrmp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iojixwtc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ldyifxlz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3osjqhpwe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fdqphgak.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdqhnls.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3thsnosdr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tvvohjac.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbksizzs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3omsuedco.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xvpmlypy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gzpbutvy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttpkaldz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rkwspnnx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ekyuvchk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nddpjzpn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nqzsautv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbztneka.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpgzrrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmmwzjwl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yqcjfghp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knhxhhfd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlfcsspj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3phznaepn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tjxgzlex.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lvnertku.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlnuqy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cjfqsqfw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ilepyejy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fbqrtkid.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqvwifux.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibortcvy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3geuntolq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hijtwfhd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhmdnzjc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3scplvpdb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zoghkmar.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmkzcvvi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iqphfavb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3skprgadb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aiydshii.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3senskemi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qzdgtbsn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zqlrmpqp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gkddevtr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fcaeiipz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3idbvvlwi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ttphfxrf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3muudlfau.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cnnbvsud.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mylwjizq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tywgxkra.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zorfxhif.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bkdxpakk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aehcmsto.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qydnnpvh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vcugstcp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nbqnxoin.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wxavdjre.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3llifaojf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dxenpbes.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzegpzyz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gvihizam.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ndagezcd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3agnrduqd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3woxcyerk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lwtpzlyd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bwbwzgpy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmrrca.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xafdaksa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xmqoiyfi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3noackseh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqiiorqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnigncmg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jarjthgw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3quqinvka.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dwytanqk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3buxjlwed.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwewcodh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wudvwnjx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vvulnhhz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kruvavmu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mdoyrvxt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3whpzubit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rctgrrma.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ghxhegoy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3openmukp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tisivxxw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bcqdpqtx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cppgrzjf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hezoutyu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fdnikojp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhbiico.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjfkjyf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3iinzbmuo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ubwcqzol.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rwixirtf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nmdgfosr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3snqiztio.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fdirmloz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wowtgrde.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zphtmfbg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvreanbv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3isxqzxcc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3icqlvubh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xluxrkga.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xwbcubli.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rwzvyqwo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfafvvv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wimmlrcp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ihcvzfzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ojtmuiti.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omnmivmi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pqdttgog.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tzqeehfv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3duxoexxp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yaqolwqy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvaknyqt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zlfubbtv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pfrhxjsi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tkqgvvdx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3twsugshv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mcwvjuve.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rduxlbgh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogssogwb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ukjggpam.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cnyzkugh.html


<!-- 参考信息 -->