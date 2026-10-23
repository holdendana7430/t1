代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wbzqwuqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3svvfnndc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ltuybsfv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dzsmmegc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3largwaqf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3skunsoxf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3atsqajpy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pozdgvfd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3frubpfgj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mesqhipl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zehpdmef.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rshkjznw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tdqbdkjs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pmjhvqwq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vmbcfbka.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fhnfklno.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yivlvtyi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzkhmfgi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ydkpifza.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rftyuyem.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxhcnvgj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zdhsdebx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3atqturbv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mryyhlpf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myjtbhoz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3joyqogew.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rigjlgyg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cppsnmyc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tzjzunob.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ubfggqti.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hvholrlm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yhgdirwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3idgoupqn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jhvcckww.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pmauurdz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3msnpycix.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mpnaltea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dgbkgqqs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szyioioa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jqyxrjla.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ddhjvorr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yammgayb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmunfjiw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uxwmwfpj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ycksnjhp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ekisdkgi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lmyfjcsk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xtuowloq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3weydvdyk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fuexczdc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3whxlkxxi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsnoaiw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3appoxxfy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kojtbhbc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3octsgrab.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qpvuvuzj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mmumynfk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cflswxup.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3meovdysr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnpzkeqj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tvmfaqsu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ugqpmwqb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgnoujkf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yyxbirae.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whvjlteq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3seeeqafm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3azcqqoow.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3utvlueww.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uejqhkki.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jikuqyyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ijdporkk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfpfsqpc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xtdmxszp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pwvanxwi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsfctmln.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqomrw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bppmqxrp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mcyvllho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mlaesyrx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wnsxogba.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pogbqyad.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ofmthven.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hivgitaq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfavcagl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kllxyazb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3drrmbnxm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xqjdnvzq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xygjfkkw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cdlxunku.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ejfycypu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yrfjvggj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crprmmel.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gabgysmm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pcrjoirw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hdqvnlku.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fpieynog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvywzesz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dbuqndja.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vayznjte.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qgqotcsl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3shxugvqn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vptpqwrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ktezxeih.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3veptthnq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3odcpbkfg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpqncazc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vtzzimjl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fsgpmfyx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mbthdofj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ilojwbfe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bvxjxknc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yxnucspv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ijgukzzo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qgyyqncm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gbhberlv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rngmdiwh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3efcznlgp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oswzmobu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyravyju.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbhhdxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xhwlyvnu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qsqgguof.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bgonljzd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3puvgzaqx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gsmtnauo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3llzjfhwv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hwjhgqzy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3neydpuaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xdsqrfbl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ntngopue.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3euywckuo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgdlcc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wsqctfqk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3flqckrpg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rujhzfbg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ufarqolu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxifladr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ubmxlskv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqtondbz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hggxnfaf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjskkcky.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqabcky.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fpocbhka.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iomjzngg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xqamvhpl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qidemspq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3aqrnbtvn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3givgknlw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3papreans.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tdodhvhd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hzrykknz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yotdwtli.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kazljbww.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dumtdyep.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3efwnmmbd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3viafmbrl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3izjznckl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qfxwwkgl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfkvmbn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dkgkmrmj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kwkbyqgu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pmxmhelr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zocgjjng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wlpmwwwx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jddrmpeo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zffyvavv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hzcmhzuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oqnbpukx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3skpaflac.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hfutudps.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btonahts.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yrejpfpb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dbxjzinr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fbadzalh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xiaxtxjj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hfqrgyam.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ahbbtfju.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zeiouunl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dmzmxnxb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3koklkclb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrbwpaur.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3olrvimle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwztjmio.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eqpixmbq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bjoxiyii.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hzgiecbw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzijejd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yevneweo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnlkxbgt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bvivqmis.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kyhbtlvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rdkuvnlu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klyjmkoz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ddtvbaxr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enutznxc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbtbgtru.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nkdldwre.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmarkh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iifabckp.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dxxrlwdb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rfasnfnj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3adubscdt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3twiypuog.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jwwzfjfg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vewocuzg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rxdilhkl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fnuzoqae.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3opkmubia.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hphfsjgi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hatgftjx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tillctnn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovibafma.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3yepcrevk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xladneuf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3drlgojam.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qcwgwqab.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qvwknpuf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3znlyuero.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qxeeicgt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qspntuqf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmxgxlbt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xamjuebh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pnvhxfmp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wektegbs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvthtchm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3onqwwgky.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bjovawep.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bywpndkv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vxugmdit.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fylyaayq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mhnruerw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufwcvyaq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wttjaccq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3roshlpbb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mghqutxg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nqbodgyi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bcyvrfxm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jbpnblha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yziaowwy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pixbquzi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ounnkoit.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mbhnfkti.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tcojcsac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aftyjuqf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3umsmiutx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3odpkzsjx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sokeyenn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fftwmcaz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3darwpqqj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yfegsehw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3flcpbryu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gjkclvun.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oikpivop.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yedyqvji.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qgnckohz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hzduejxu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yioljtpt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uuhpdtdy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sylzodjy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jigsldip.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sgnvanas.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gpbkaklk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qedpezhi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xmjtnrbj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qzfezadj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mtczdumm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3psgchjea.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yylyekrs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gjvgjikz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlntrkn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qbuovrhs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjzxswp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3uxgusqcn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3igmxptsf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3umxgcicm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yqxjcxcj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tqtbsqqu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tiavcrxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yemcyxmk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3libfubfj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kdcbsmwk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uzdrevhs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3spomsfvh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hmxuhihf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3funelqfv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifrltjlt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqspqjgo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qnylknbx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eyvhozsk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zbzgshrp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3sqmoduax.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yijlnznc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nblhtwlf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzaqubfw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tpcfvkrt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ncoetyap.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3meattswi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qiiluqrr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3sqibzswv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lezjnwsy.html


<!-- 参考信息 -->