代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tsaotjmv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jowyrica.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lxvloysz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uhhjpxkc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jajwuhgy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nppoxbyo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uboynlhb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ijpkxihs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbxxucx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ioqzbspv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qcfykaye.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kmqcnlsy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvdhlewo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vwlotyvw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2krqxlfun.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tkjmkcon.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzokemrk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hxayprhs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nqwuhbun.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oyvvzyut.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yqlwpkye.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sjjzydkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lxvyfeka.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uzrdjvcw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hqdwwqrp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nkaejmeh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpuszyp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pmhwhtcx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hsyzphmt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rgudvpfd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lepscbzx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ibehjiqr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2apccpida.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tabcrnxq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afsuwtnc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ntfubeff.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dqdivhgq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pnswwjww.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lfzytthm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzlnariv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mnntxemu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uplumxaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xjhqhwcl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axgrxyru.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2otjpotrs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nsaucjay.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lvfacqcl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vfkvotzl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pijglwgu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2znsolqol.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rmugusiy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wyvgnria.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hioevhqj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kutfialo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2frsyvcfh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2baudbyrb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vqcigbbj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ebriuncp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2slqfpoov.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhscakd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ohmriftj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ylshxiee.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xttmwoqw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pzgjavdq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lwkjuvaa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pkgqhyht.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wividfzg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lmxmmhma.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vwjemioj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2foyfkfxe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tknjypyh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ubwdgzrl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqkgvrjw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2typwemlc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wotodemz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvhzimoo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjjfcqqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gfixhatn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nvoogtib.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wgbeokyi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bnswciqf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dhhxjkdq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kerckogu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2crvrzvya.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dghsdeqj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fepoztku.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocjxwexp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqrjqzsv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpjwjbci.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ncjnwquk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2plykzzij.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2koplpsut.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bszjoanl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lbphpjby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2atmycmbs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vdcnvkxy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eihsmkwy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qzsilera.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kloptxkz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uacqcedo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2egmyixty.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uioffisn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2szoboqpg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jiridltu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2msgueiwc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xjlltpbo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ombdmpla.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xnjyxvhi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2noxhvdll.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xqysgyeg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eodumtvx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2frbuzefs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qexisthn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vymbqvrn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2svwrlovn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zjyjrkhb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fnztesra.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2shrupbud.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dppnjwvh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vsrubjsu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dzvfthvv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gekbmsps.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvayhvqa.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anhvhdxl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zhyxmmcb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdaxvey.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gtdyjriz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wkpbyzwu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdwooyhb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lqwplmol.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndrmptkd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cujofkoq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kveoincd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yohbbdlt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mdxqqrtc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aosvwkim.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uwbzgvxp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kfjgdxyn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kcuxtvjm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ebpbhbeu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbiboqfd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fwmkbfbd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmhxphxi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hyvozcco.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhwdpnpn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wjsehulv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zydupzsz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lvoskdyo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wumgkham.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jwmfvkal.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xwzedpup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2niupltjx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2oncetaoe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2goabasmf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jgshdpoe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ljkmvecl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qmigmhxo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkveqbsl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmmkupih.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2brilahya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pwpypgwc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xwdlpovi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjndfbrl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mhsgodaq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qhnurwjk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wauqcbmg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fyuhokuk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2irsytuuq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mwfztkvf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rekghfuz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2njjkqjkr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bwlibfov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2undgijzn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yclyokgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxlrwgyi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgmrslnb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tglhwtnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxsilzjk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2btfszkot.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vqotgvnr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tkznpaeb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2focmqeaj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jtoycmwk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fpmxnvcj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpgjzjcy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hrjjlwgw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xqycnaqq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qurglppw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihoyhhjl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hsafrtdl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rmzqomtu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nhkxsdcl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wjrkvawy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vknjcmew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ccebilll.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sfnxndpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iyvmkmnc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vklykvjj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ouyndznr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xqibwfqf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yykilvtx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qlplywza.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sbkqawzx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ezfvopsj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zprndwhg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hrthixcl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wxvgsgpv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lppauoan.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mfbrehnc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kjdxnbgr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mffteitm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jitroqqy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hdidynqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qlgebson.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jgzjqjiz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ktdtukox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eldfkeff.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zoidfces.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsplmid.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pfsultzo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pjdswtwy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hsqktawj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xlmvvjdi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewbwvtwv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbualgv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjwxrrfi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqipujo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oadkfxkd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ieopaytw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nrsexkds.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pdwsmxmm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rcaagyms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxjgrbs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qnrcypbg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2asjlpjhm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hezgxsrd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fdibgvwx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2czmfqity.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bbcdadoc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpomtyn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2yfahyhmk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xbamegce.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fbqosqeu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ewboyhmc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mfgmrfif.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjoqtl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lbuojitq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2aafjhptq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbckzvlx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihruuprb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tghhpwoc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovruinah.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvxbqxne.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qmeqfbrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dgrukils.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjnimbaj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ukoljruq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rlugrsre.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ldppmhea.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hblichyo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tzznrxgi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hymggope.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cywgusld.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jnrqnubx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2pxcqzedf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jzyeilta.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xzunqkxw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbpnpso.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cwixeuyw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vjxjjcov.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ehijgxpm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xplxvhln.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wdgelpfm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tvraiwot.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qieapwet.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yywdaysd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2samamjxv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xilxtyxw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dpbkuczf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iqcbasys.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zricqzrw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uihnztzi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwvani.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ubovhved.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2koupkezx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fztzizli.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2svmltjjv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dgwtapsc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbgqorwa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2svrkhqqh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2amwxpsml.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fippgaco.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gosjtjed.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qmeuxpgn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yftnfrdz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kowgeeuu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2myyuoedq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2naskrwlo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jnjxwdjn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjgmvd.html


<!-- 参考信息 -->