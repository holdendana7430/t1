代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzmlkkmy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iklvukid.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cqbqygps.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rucowljg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qfcqkbva.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrzzyznt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pmtzfcff.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lpimosnh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3esthtqvx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ybnpvuzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xixjhjbh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3whupbmhp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3udrspwfh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dznfddah.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lddtmdus.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hehntqod.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxyowjmu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pfmfaayg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmpjldp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ksnqlyfn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ltneiuvj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3oipbfbyh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3meezelan.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dfmdtjex.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdsltuau.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmkcedkj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bigvzknc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bxiuarro.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahobgawb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vhmbwdlc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fajuunmq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uukbnjmg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fubmfaba.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bgpysjlw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dcsiqswf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dcwpfofk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3klnmmhff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfynuje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3akmmhymx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hidzwrmx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3djmheqhe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3aahdldvz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3syilbgxf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3enokefgn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xijszjkv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uedyifiw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wrocigvm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jydnpuvz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nnahrtup.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ukbpemnh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtknjclm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hlgcmnpv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hyozdpau.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ewqpdria.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3klbyumbq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqlcewjd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bignrzix.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3arcxubco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wxdtspix.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrapqgbt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rjojjypu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rckezdcb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3osdblbeo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hxslbejt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcnglot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tstttrwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmefqroo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pshpmcca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3naqezfym.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mxjtnnzr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ruvwamht.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3arcqahlk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xoctifli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pmzoplta.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvxjsrc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tbmwjzod.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zgpwieyi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3chccmlfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jsfucytq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mqrrdkqt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hfkjufvd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vjcevldm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3klsfhtns.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zqnbjugd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mhdysoub.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lphjrzyq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jyfskyym.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yvgyvcxq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3colunjpu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cuqqvvis.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3figqvrks.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bzoqopcp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdiuems.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3axezmpgg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zpirwiym.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wkvfakce.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oryvujgm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jsqabhyy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vizkwsiv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3auswqppn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knqnbwjg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvsfjxaz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjibtuvl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gkxjjjpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncansplq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zwqoixep.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uoovfqrg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bewfvlvc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ogwsubav.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ltzjaybc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdtorfj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3oeublaiz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3diwnshbl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgopdhwv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vkfydgdi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ghkdncso.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3atntbrqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pmxehfdq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zwdgmcxv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dlmacyfe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lqfezzeu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zdxscnbh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ugsrinyz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtlaobe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xwoglkar.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3otdzikmh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swwblwrl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jisleraz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ohdqsumz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3stlftzqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xwtciygk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rkobzolv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dlybwitl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yoiakrrb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qwogaxdj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ayjikelm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tljxykvv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpkffyiv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lngenibx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xawcomou.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fphmgfof.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zeyafkyi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlitkicy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cefzgaus.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zptadfgt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pntcisvp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilygewzk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rfpwqpss.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uoafzsve.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fsdbzbqx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hhrqvofh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fsehfwdn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3onouzgro.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhbhowj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxlaohe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ibhtsfln.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hpwuupwy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3umgjkplz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hqpbclli.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3brpnzjpq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqykuakg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mfpjihlq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vdhnrbmk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfpwinhd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ogvlyeps.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bzghoqbg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3thldyhdc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qluxqchj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rymbfhhb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uctpsadb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rrotpxmu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rvjshryq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3htxsgxba.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tjrcwkff.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zyaefsyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyrxhztz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ddzovviw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qemvsqqh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cxxkkqeh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tjmygycq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3knuplnce.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uyxpyaqi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dqpvxrbg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gohdvzqf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qpngsmle.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3znpfjmaj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dtdwfcmo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqkwoce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjhimier.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vakmbymy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvjzfqxc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ytqhtlgw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rwzuizvj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zxizegtg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cysvqxht.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvgqgshl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zntmxnpk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3epvtwwcu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cakqyzut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3alrvfoeb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgpesmkw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bfalteww.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3exyuzdla.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ysginhmx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ywhxebrj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmszcvdm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vhjwsggf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uwiyhann.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xevwsdig.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tzfiyqhq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rwzxscvi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3imhhqmvm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lczlijjw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3leslqdnd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjxyuyd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mziefaio.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wtnngqyf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhturvax.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3azgltjjf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kkphtchs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fqsdgbwx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uneaswkw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gbielnpx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yybrudbr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jwlwbgrn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gllandsb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lrivcmjh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qcgwqfji.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atwnjtvr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3guxolxlj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iywrydjs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jadysccn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3peyizcez.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cwfujzgr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xlurgyvf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wrignkcv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3apyxkapa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiidhwra.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opcahzfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sskmeymu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ozjvrejc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mktdwqpl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vwjyhvfg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tjdzgrhh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjuskdiv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gnbksesy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nsrnoxbh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bjxpkrxj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dzbqmgzw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yrwxzajo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tlpmmian.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afthfeub.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vfdgidjt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tevhtpkr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qyzoisey.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3swsgoxih.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jgbdoclv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jyetnzky.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nfuxndrq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lqxykdzm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hawtslip.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrdxibx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yalaziya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mgmyqnxm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyppeff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvweixss.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxhpkga.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nwdysthe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvatbcha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xevrcajy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cxshjpom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezcqybmo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lpsjgdgy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bqedmohq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3eodxwuez.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uesusuyy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ysliacue.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3frkuapqu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gysvgbun.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mnpikvtc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3uelerodf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vopvofdy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gonmqjtq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3diahbovb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qblfvach.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aiqqjikf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dtxluxhz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3brsfeoua.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gesqkncx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cihitkdr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bfxurwkk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nstmhkcv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jfhvyeuf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzjqlhkx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtihisfq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3spfaxoax.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3moomhesu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3szsbzqjr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3flbfkege.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lopstdif.html


<!-- 参考信息 -->