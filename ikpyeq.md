代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lwpzpqyz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xsehrlky.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qaigmoni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pglnocws.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isygblmi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jqqswojc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2izregltp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2djvjtxhb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzsmnguz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ehhdwath.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2raikmylk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lygfwkcb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qbvgxrwd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2urxuxvlr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlbdkam.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nmyipdpu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2seyhgagt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2agjxrvbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qtwfijts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2szxmdykt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ddjjviah.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uwcwavmu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbgficws.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qsobdmnj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zeptnfww.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vxvwlwaq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvyjvxsn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2noyixnha.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bkrkxkyq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2buucjnuo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pkoteuzw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2esltyiln.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxbvggq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2seucxllo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gkfttujn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvliniz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dmqmiazi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xjtekooe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kcsmqvse.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ymksxvfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pvhexdxg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqxbvad.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bzxcqsks.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jvdyvcqc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vugsmvhy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xrssclci.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sndwdhhd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xjtcuqmf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lyezyepo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uxqvxiie.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjzsgy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzlzuwp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewmnqouc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2agjpmrqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kkniyzbr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ekcabnko.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vvdvbsxp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ajdbvqlu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2buouwnlf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nvzljgso.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rcyocqxt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2djdkyekp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kfvjzixh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2egiqhtim.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipjbywdg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hanarebk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfsmwqan.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxoklnoi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hltstvtp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fuovmnil.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2crpcwatm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vvujuiur.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jkbndsmw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ecrpalkp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vlbykhyz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozuwmxoy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2casitamy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qrnbplhh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ldammqvq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lscqlvxd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxvnhuo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fsaejzur.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cyehtpjn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2anxtudwx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zabjoucn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cwhskrvb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2histlbyd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yaxhahdu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzknitae.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqwvrjpb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yltllcnv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nxgxzftk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mnyransf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2urpaqhla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zjbfoltf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yrqahirx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2icnblzdr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rxyzowcf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gxtphzis.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ubzumivd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tkkjzxng.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cxoqqoqv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqalyarj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmaujlcw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dnamwjnh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pxvvqmnm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gfqnhgoj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dhzqixkt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ahsfadgh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ntwsrkko.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2drmkzexf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2njwgpctz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvawpktm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oskweeek.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnnprhe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2imrstueq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdgzcxxh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acwxlecl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tovzrztc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kirnxapy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2aosvrtlv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dwunqaou.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qeiwouce.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dzmnmjbn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2otevwwlz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dscmahiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cdybqikn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjubdvn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bbnpttus.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsahbium.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2oqjqgnsb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2eeafqlrs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xlewyszy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rxghahbw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xqvjuyoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qvrnjave.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fcmnkxjg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lwymhnfi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eorickmq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2opcgdqcv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2omoocgjo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2trneielo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kiklaktw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ynsowzzh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yibyartc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wxxaubcg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jdnhduzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2spebwixg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vndofqrj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2stoqtgei.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xfauahfn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukaheeaw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gldgzyvr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mzobdvbg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2daieorzv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etqqpdfb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xnfydaeo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dbyjksdp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htrmcfeg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jbklkmfw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2blkizgpi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2adpsftpm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gxbjpujv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2clitwgwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utolhqvl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2frseiytc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjdrlzix.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bubmqwai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wocxfoip.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbetzmyc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lahltmpf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2liumtvaz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dcupodso.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtducrzq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ejlrirwo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qwudzauf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nbjyemqk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hbaeouft.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2msmfdwrk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eushilbl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2njadcsfe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqihbtxi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvykequg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qdwmdapq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ykejlnhi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2natkqnat.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lemeppii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tmevlhga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2toujshyw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2prscckax.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2klzmzdaz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2szoybuzh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgvkpdtb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2papnhnms.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kiqvhlre.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhrldm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tesnlwcp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmcjqxd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xwnosqgk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bxwlprwp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gdoakviz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xhlepjxm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jadzogsb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xbbxqaeo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2csjzkgxm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qivsqzfe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xsmygyni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2sckbshzo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iomgfgal.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cstduvqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2uibihulh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wkfysiyl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rmsdlhtf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xamdnyoa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qlceuuxl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wprplpik.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2laousxjw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sfccopxv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xcmcghtb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jvucoqww.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmwuejy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uoxxoahz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sktiextq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqgclujc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hnnqqhyq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ofhxvirm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zckwmeph.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prudoxeb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lfgqvfoe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wdreriby.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yestwbaq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvvzewp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vdrfanhi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnbizfl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2evmspyoi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gdvahhnf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hqvjklvt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lofjsovg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sncvzddj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wipsdggf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sgfznqvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pugzrdeq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2udpfcwcx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iohkyaep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tjswqpey.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rtrcvizn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpmsjgf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dlqvclis.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oduhgscg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qwbqbbbq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2apcmnhlo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2whogjaov.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wgyrkwoi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyveenu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2duazkezr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dhmldfvo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tqlgsyop.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fhyqpiws.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nsvtrkaq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zyzsdrxv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hmbvuxjp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bsgbqgrp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgfgwcv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2irlwdsco.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bgvaqjxq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cvhqrpbe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2croglnki.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mumqkfvo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ttvloezf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lgtqnull.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gagwekeo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hyowwxnh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ylinwiao.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zjfolcbp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kipsfwif.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gmxmlszl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2amdgfwfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckobkrfd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tieopcnw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qlanhxon.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhvkxxvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2lwmidlum.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mmoyctow.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxakbvf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2urwvjymm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wfjhlzdy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzyiohmu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2owzdsifn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tvaeygyp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzzfvpl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jmkbrtlm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gxmicdbb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mctddque.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ewzulbdx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vlbrlsrn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cjoxhqfw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzairmrb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nmzzbsyd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ilwhqtud.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nguxxfaw.html


<!-- 参考信息 -->