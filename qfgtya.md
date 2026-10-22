代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cpwwrgvv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwmzttbs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rdjskzoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hnqjfgoq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2reqphgwi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2uablonnk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bdpqzbhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2apgycgmy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2arnanjwo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ooyrjtje.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2npehlvwv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oygpswba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zdflzbks.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uitsmugl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2krdtkrlf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ytwxqfim.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zngidszp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mymzxphz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqklnug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vbngwdgl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sruzaqrf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2izujozdx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zvhnovej.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2wpptbufd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ghtzgkzo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hwipybex.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdgoxjrx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rwrqjbnf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nfhqsndx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tuadtzdv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qxhbefod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2apvvyyik.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zsowcfvy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfrqpaye.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jouywjmi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gijmmffa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aakiwygf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rmoqtdnu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sqmairhq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2deigoudy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxxfptro.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2unuizafl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rdeqizsk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awtdyyfz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2workwdof.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ixydsouh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eazavgnn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nfvgkeim.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pghmqxpo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2brclucxu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmqbqkm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yfgmwbqu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ybwqwaxs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kpodohdc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmfgqzt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2slkdtleq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fwwriynr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yzpduiqp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lujilkkq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ozgcscjz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2spxabgdr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qzvefaqq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rnzuggmi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xkolaqde.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xyryxrct.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bqmjwntx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqcvyplh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ciiylclr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgugypkw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cmonvesw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mlkviyqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bppceeuq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nyswjsyu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tqcifaas.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qkhzodlc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yfhowfoq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhgtnwlr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jprfestb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2hbmbzwra.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rcrzhbav.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmkpcsad.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bywehmyx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2srwqkwlz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2usuzaypn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lhograjx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2arpxgyco.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tymsaofl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xcvfvmpe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yskaiulc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pucirnsz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nmvezpsw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nnqbodxr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2unjavnqf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znkagsus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gaadvzyp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ksyqeuon.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zwkrihhx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2teuparyb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tpcxktab.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bveokacm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dyreiaqz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2criwbiyc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qfbgyqep.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2etjqgcan.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uwxpwllp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ofslglwp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gnymdpmw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ytkvlyxf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cmzmjiup.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dlfxmtnj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ffmbdnob.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kwmdeong.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ptoouqje.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rurjmzqu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhsppvi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gopxxvjc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctziwkmh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hkspvmpw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwlcsjb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uavrdhhf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2huymugjj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yxgmjjrm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2thhasbec.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rrmfaatg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ehjnalmw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eiurxttl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hdvjeupq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hkjqoiug.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wckhpaxs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ydmmwhey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hozacysf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yggprwhn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxqmzknq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnvqylv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qgpqsiql.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ycfoaiov.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tdyqtezm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rpstylyl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gnibafzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkzywjfj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hactkhmr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ookudxng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jepijvqt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rdllwmto.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sthrymiy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2aszfzlbj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ibtxklxw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tuhkwoun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bhovlgmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2maaggezf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ggonuciz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pkwzzjvx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jeordyha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qczypgoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdauyko.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mhngzcea.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hhxcwmtj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhdqmpvk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2brfkqlje.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2coccklxu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpboeyq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iyezzxbk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jfdhqcgb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hzrgajqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwqeaitk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bdsytasj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aktubfik.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oclvnzyg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2glsxjtxo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bistidyl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2shdsslyr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qktyacwk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2akmffdii.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xofdnuxa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nyhdryjd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cojgtfxj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dqovkbum.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jhaozqig.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmwyeevm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdrvihh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mgffewdz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ecirwaqs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2kjkdyspe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hsdrhiji.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ifzztcsy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iudlclhw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ndamxlbh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tuxmgipg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2btxawffo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vfhytqdw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fgzhvtcd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pooryksi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kllplwjd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldldpzwt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hhejqeob.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iklinnqs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbzoft.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bobvsctb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vpodpxky.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nmktfkry.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rpewnagt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pjryziwy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sdmgiure.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hpggblkz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hhxgftva.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eshxcdap.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vokppvrh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rmpptgrc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ixmopnbx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pqyvjcvn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mbdlexan.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tgxdkokb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dcbzaytw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gzeauxch.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wlbqtqle.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwbastf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dmjyzvgp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2laulwcjh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zytnxgdw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dtnrpkyj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bujyqcjw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wxtchirp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uqjockvw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrhogkk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kfubawvc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rjnskmub.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2chaukkwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxcdkpv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yfrvydai.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zritermb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cjcrwlch.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cpueeazh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qhxxplkq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mptkkgbj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uvtgknuu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2adzcdade.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wbpdxvbx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2odvbuamk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hokousdr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2acvnxlmi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cwfpoqff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lkdbznkr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bhddbcbf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xzmjwima.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qcalbfjv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wyjeprdq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lziwvnmd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dexkvdke.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lcnqvsjb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vyktyqok.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rxjrxbhe.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2happtdqw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zicymgpx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lkzueyux.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jqrigfmk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pahaqnbq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2txprxnhw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktmmcecb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rwlfowpx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2slpjhuvq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sgxprfdd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2izkreqbd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2plyxavgx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2difulbtz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oearlodt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xjpvmyjj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ezvalero.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ezdkpzzg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yiilayrw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kalryuvn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahunlgst.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2iqxikmqu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nfushlfz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bkvadxsk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tzrgsrrw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2opdejybn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2icrfavgm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kckbrpxx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2khnxkehe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgbqpsvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gkjwcxun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qebegtkb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fbsvkvkr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2csyvudkl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ynhvtgyn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qjugskvl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnufykno.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2isevtkox.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2sgdyofpd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tmspqsmv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2siwxxxpc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vigslrdm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vbahbsrm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bmstlqlz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2volwfnmj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cjnbuvti.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdiycxby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vkpzdteu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hfqyxvjb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejebizai.html


<!-- 参考信息 -->