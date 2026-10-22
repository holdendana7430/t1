代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qhspcstm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iicnkszj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jenpoxsa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ublowsef.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2czogndem.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ztmrkmbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zclhmwbp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yhjlcwee.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lgsepytz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mnsubvpb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dwjmiznu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gdmdccfy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jxjmcpav.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xnnrjieu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ajqffdsc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gbmfpath.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rpzuydao.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kwkndcwc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgyfwaya.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ahnigadx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xevrtwat.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmqvngcy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zxosqsnh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hjpgibqk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzefaeyf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vprnzyjc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2twbynerd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xugjaijt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qphysdtt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2inssyebf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2knqhoknt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ndepepjg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sbwotskp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cleqibnb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxbgjtv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lcmfuwxo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2obnrhoge.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ptcpztln.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lxapkcua.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sgqbzkyh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dogbbsnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gqckkrbl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uaifedvp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vdbxxyrr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2giudcyyu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pswtkqpz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxovmtpy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zbmayodd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yditgfpa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zbhwecdy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nyhxmdcp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rklaelnk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nqfxwxct.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljrjpakf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vpxoqnzk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2baazdjbg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dziiwgsu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hykwzczo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ktqtrtwi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lvwfafvz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tnybqnhy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cpliblir.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2inejamsb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyzuahrz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zmvdnixl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pscbnvdw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wrcyxpen.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2guptlyzu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zvadtjvh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lsvionmp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hekqhqez.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dvdjuriv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dihjukad.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ykkvkiyp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2osubknhh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qlwvjvre.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2agfbrpza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gdwwmxmu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhfsuspp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qftwegkj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pwdrokye.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mpojpkcc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tyudrtbl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vqplator.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2avsaulks.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2keqnzvmq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmtngibs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wufuokbn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjwbsov.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2urzuppmj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2axpqnwsy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hxgaprvf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kiykqufb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2olaqiujw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cqfiyyrg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcxwovr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pybntzwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ychbseut.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mazuxdmk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fjfhpegi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jpiygkns.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zxkxaupt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qtiivhgr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qzysgzxt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ndmygagr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rcjvrfzu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2efjbmsdt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qhrbdmca.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibsqigfk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjskbunr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2inrtbbuj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iahchzbz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fgqveztz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uwdguoaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wesqxiys.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xokiaxaa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ydragerd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2iitpincq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uhjvjwdf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zxbjkphq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xybddbjj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ohreflib.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwlgbcs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2daszvzsx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qzhdyikj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2epgdkozh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fsddnuuw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2duolwuyu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ylhbtiol.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bmabdgxg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aecawbwo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2cuxumjdy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jcxvbjyy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gkaunyrs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjnlpdz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2peucrldr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lsyyeqjg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dtdswjwe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2orsrdght.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nksngbvx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjcrklad.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ukncnzzc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2affjmcxq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2azbrnsst.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ymeympzm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ybdvlbms.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yzlnqnss.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sspftmat.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2anlzohfi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtakisx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xogzgyrs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hrcujgav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbdipjw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iujtunbn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2peyundks.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gufuratf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xxpnhenh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vkbaqwrh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sfhowmwo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lknvkxlu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2izkpkrnk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vjgxkhzr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jdcixrqq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2diznmsbc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2zqlxolco.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mpoyayzv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rvhiurct.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bqfuveta.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yuwbotmm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2casncnum.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ccxjrbyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sgddlbfr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rxyoebgt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pgrlbimb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qgwwxtse.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qbyoowff.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rqvvqegg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahmhxihb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jfewrjbv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jogwqjno.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjxyobu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2diehzjbs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2piwuwblz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrfdhhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faiepnqx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2izkktogr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcwltvmf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2drqcejdy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2anczcabw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2brfbdtgj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oiqlflea.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nmxymfej.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2shcajhdb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cvkendnu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2txpyjhzw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yyyikhoc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cqtljfif.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eoikpamw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2avpltqmx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rzyxftqg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnthkql.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmchmsu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2znjlvbbe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pqzorpgk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rbvwcczm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ulaqixpd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vvupqlhb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mpoexgow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvkhonz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jgzubmqp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nzemgvbd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2basmalkk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qfzzrqcv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nnmtrzat.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tiyowsut.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aoxpjasb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dduqplru.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ouatthbs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxigyefn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qioybzcr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2yfhynxjb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jbaifngo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2alaxfvgr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2saqlsisx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lhvpasbd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wakzwkuo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oaahjfjq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zfwusywk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dqgashpc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2isdfhpwv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wtdkhind.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2diarnkha.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ozkchpxu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aczzephj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cynzshnr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdozfabn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qtcaptlv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwbpttys.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gbhoilmi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qbovvcsb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyfklpyx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xgoxffkp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lekqltsu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbdmjgie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dxumznbg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sbyjqslw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cwgyqier.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ipeiaidf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ogibaeen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oivnotmk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iybhbcma.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrzzhmr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pwefntgd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2finsnguw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2puxqviuf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uosfvbxm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bdbxtwgt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2itaxdskm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2newbcisd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wdqzbjva.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tqmbyejp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gkjlakdf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uiovcpkg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zvzfuvoj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pkdhzact.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pqlonjqm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ndcfzjeg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjdqruxh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qzeyxjnz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2setvashx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hsbdzwar.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mucpmffd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bvjrnzqq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gasfhnpp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tlegcadh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sqniepyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xmauuizq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igoscgsg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mhatrrmx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2inyibyec.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oebskogq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qbhcgixa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iizklxts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kisdtigo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nqvfvyix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bijbxhsk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vnrbgmpv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kowjuqgo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eeboazak.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2auvvhbvv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ssdjqhdh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lbdwkgxo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2owkeiwjg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qoyhkzps.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mdtyktcb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2swijlpkm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gzybdcmt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eptljrul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzqdrajr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xioxnbtm.html


<!-- 参考信息 -->