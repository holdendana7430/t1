代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aamdjplb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pljiqqrh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjjpcjyv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqviae.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zrvczbxs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3avysvudp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3owvovjqf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uhienkps.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qmksvlcq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mjuntajh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nhbnxrct.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dixhjqnl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zagbiqgn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rnomyrxr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zhtjrgpc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tyznqfgp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjbifmwm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nwrqiyds.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lukzaoso.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qsioldat.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cfuzprtj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uvazseko.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ifpprypb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ocsjtqia.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmyzsrw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yexofdmv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3oitbhjwf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mrjzliio.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psengtgy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3sdytywwz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ekzlddkq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mqomyisd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nflqfytm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vpudhuqp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yoxuctea.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3udogbqoh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vtqccqcy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lubruqeg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sfiylykj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yakplkga.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ptqkoaqy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rgbuiwtn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vtcskvhi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jgfwykne.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wicceybf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3icbvhudz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjoiyhys.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eyegsira.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3astnikun.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uekskzba.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqvsvdox.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3siwfwuec.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3weiegiof.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qlbvqdlu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hluubaqq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kgoacuxn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ovxacbus.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sdonaqgp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3onmgqzom.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzaenmud.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cjmlflcb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bixcrsxx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nxwxmyqt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jaigqrmd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pqojxwkt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3civsbtrm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrdafrg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjnbuxpw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3iklsrfjg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lqvydvpx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vphebhdu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3drnlhruj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wptrgohc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmabpai.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3alcpfenu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3udpolyyr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dvockeoa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rkssfhod.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqpkfbl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3peqzybml.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xiqzyazf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3orniymtm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kfiepedm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aubfwvcm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mwcijcfl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ralgnlmo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iqhvmplc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lqrfyiwq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3woasbwwo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hzoqarzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yipdzohp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cedudhbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bvngtfeb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tpwmrisn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bdquhpdb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3axstuebb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3sbxuosed.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fhkfplxa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zmnjfulu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldcilkni.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wmgunlei.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kzucwnid.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjxlxbcx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vaxioggu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqksspe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3fpabesqf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jqadedhf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uslrjebv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gjyzoijf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbsbilo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sjhdqohg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wogtsciu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3siktfsye.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qddvohhw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ombsavlq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgroqb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gwamwwsl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hyoxylrh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qauxfdnh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vbpioqgg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oomtjqys.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ddprkqun.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lhjtuysw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yccznror.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jesggcsr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xkhgedoz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gailjwck.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwrmzyj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xxjgouwo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xkifugzf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3loyzxyve.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wogfbtwg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rqpsbnys.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ytmoqnqb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3iqfysrcq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vuebrerv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wibawbcb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gvnsnjoj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3trmpasdz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwiyvefl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjbwghq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzshvtd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jbzjylqw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xfkqctly.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtytxcpx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zkkwnwwu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tunkiawp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tohztfcz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wtpvyggy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ufgagiwh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zfzqzhbk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3swuhztkp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ckirxzgt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnwpkkr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3edyxgmle.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wzczpywl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hwovhwqw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdfcfer.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3llxbcnbw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3frcsetye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mdfkhwfa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pcnmonkj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qjoohbma.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zhoglowq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ualaycap.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ynxxchgj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qzujlguo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gjmoanrj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qhjrdlyc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fzsiroij.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fgtgqfww.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kourmuuh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vaqrnnev.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhmxwamc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wuldyxqn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vonqgjka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jcfkugfk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnyrnwz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxngwty.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mkauukwb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3omglnvfn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3klnyfwmw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ufyzribb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3leeyudsb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oodrbdjd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3edfjnoaf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kjmyymoh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbjbked.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eneqtahd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nrwogxiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkugzuqu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nvotjpmd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mgcysisu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xcxztauc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bzmsnsma.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lqqhztjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jbwwxyzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3biqeypwv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gdluuwaa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jngcdvac.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3spqxaqxm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vzgctwta.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uszkxqjz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aypdzcpw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgtpfbo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ecodwghj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcpgcsc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fiiibzkw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ezfoglhe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cibstfcd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ogjjskii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tucdlljt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hulabbsa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ynainuyy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmzvycb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gglixaza.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dbdfhfer.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvpwysl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kdkvhhno.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3otojcujz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ppmpvtxa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3khfqbogz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qehnbukn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uznvrfni.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3reimjmzz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hchvezux.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3okkogtev.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmzzgw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfpraqr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3agcmsgch.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqqcmzqv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3oubeweci.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bgjomboe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bzmmvegt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pvnzbxjm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uidlyxje.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ktbtdfdw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cypxelek.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bqmsdjye.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfinwrpy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rdtwspui.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fqdhsqlg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cpkdoanm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ovzdlnis.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ljeieipq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3szplucpa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nrbywfqe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzlchswi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ltegqhsf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3soowtgss.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3veyhfvir.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uigejakg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tmdgmgti.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xmndzfgu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xtehpgkn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ofgyagfn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbqwep.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3plzgjtsw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qktyajqg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3motxkasa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3awaqvszb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sgwobnpl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yjpadbxd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3sqwaklhx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lngjsjiv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3haasvfik.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzqtuwi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3todgmyaa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndeggios.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vrjkfrrd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqhfspr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ssljtqzx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ymyquakp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3diamcmsx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cjoqbzus.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzdlbfv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nqnutxrc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pbbtnvnv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3couzlioy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3abhgvszc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vqgkdoiz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjnyfjhs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3blcbxjnz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vyxvclrr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwixebu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nfrngejd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dhuwyhxq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bbhosqib.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kidykjtf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cdunhcos.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3meyebkuj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dhjiuqie.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jmlzeskj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnbtsipb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qwwdkbzo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3valuilbr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3grvatoel.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ukiurzgp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gorqcwyc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3owisegvp.html


<!-- 参考信息 -->