代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jcqnjsxp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ozlxmhcx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vjsixcsv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tcgnmjbu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyjbwtpb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdpmxitq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iaafeayn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2obmpovgd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pruhmais.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqdlrsfm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zavlfetg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fbfptpdy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2oqzkalig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tiahynoa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhczortm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yamzluii.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wtngnlzs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oaacclte.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2phrtzukd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2azggcdpp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zroviecc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rnobtfiu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2smxltphx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2brfbkhfp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ukeljnei.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ivnvxwut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wsttrtgw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2awtkdlcp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nvniaiob.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zgacxpwj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ykvadhdd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tqrvlwmu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owswxsyo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fcgnqxuv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cgiarpcl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2altlkobr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spnpowjm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xdwnkfse.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pupfvjun.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ebqvavek.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mqmscsgn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qtlbskxz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jiplgjxg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yhsupcki.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fupismmr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hhcxonyx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2verncuam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eytkvnpz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2owqrnzaj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lkyuxcly.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bhnfzplz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cvpttodr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2moaqckxs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtbidrzl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhmbtsxm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fnwwvazx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lkiobhjh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2htudnnyz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2odoyfedw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buqplzgv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dlvubavo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rohwuscv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hcufpioc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwzemuq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rivvogcz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2dktsrdrb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tpjrzipt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jpspikkr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rptnmxbz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2czxsyyxb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2drpmbxpx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jcxexqdg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qfxwoxtv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmabtrgc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2laysyubi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uhznsgzg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rmxmankj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krrfbjxg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2oadzcmmb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hfivowjg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hltsvbmz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjwwyqgw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wrrhhezt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uypcurnr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tqpmmrsq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vddgmomt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ecyxysrd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2myjqpzsj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jnqvzieu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wrbgcnyp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2avcairgb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2osfbpbni.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzkaadlk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vojgpwfk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nppsxtjh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hmvfzdfr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtxjnttq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cdgxivph.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kxcpbqee.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xczdpndf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2slymjwnu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ujawxelc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pnfxscxd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxbadsg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lynxtdvv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rekijeif.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2muzdhhgu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnpbfw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spkpnlsc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ywirekhn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cbpcdkki.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wrqszmbn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qmwyeuoi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kggnlhiy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2onuvpvya.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2sfpjzzjw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qyaevvga.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2osjmgxwz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rzbfpqro.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sloujqaa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2juxjgeep.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zxseofev.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jhnxsfcr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bomeizoc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2filwvrlo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zlpwuddp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jyxbjgpg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fxmiemnw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xpuchyqw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jwfegmju.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmslrcur.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkbwrkvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xamtbjfj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oiprvrzm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xtmtpntk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gbhczrro.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eugnanvv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ecilkhoo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hckymksx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uupnwlgw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2efujvqwo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hznwywzt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2anmoftaw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fgkqatav.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkctvwsp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eolrjksi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kfyrzkbk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2yfugxtjc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrnymno.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2acmolkhv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fyoiewic.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2eshqrryg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xxpsgehn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jelboemd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jihovuzy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kusufpeu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rumtqyrx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2egfhlzrs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzoirdep.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qhutausv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qletzmxd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rszzouzs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2frfjalqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tdpggort.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnfrgmu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2audtdlcp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgwuxwd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lrjtezpg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2idspgvrz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lluupnak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sqvpiwqx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rcqpzyyl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2huiarmec.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mlpzuewz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qvmsotky.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2clyfiooy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zfduarir.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bywgfqug.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzkvlczn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mpvshvla.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2twuslapj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fidlwfpi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epoevubf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqgvzdnb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2leiasipp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfqityvs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rqhnjeda.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ibkwfkey.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pozoynjk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xssfxsxh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tzirjbfr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ryulbxhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmrqjwrn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2irbfcnmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2voklxmkc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dboojuea.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yzikpepv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lwyoarac.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bxvrdlac.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2skimxfmz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nkccqvuk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yrserzlr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ctgzxgty.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2phfrebzw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2czcjultr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nhzaevka.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hajecqbw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mwgpkrni.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gatvqess.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2glfxtsji.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ljroiiyy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rvhamoat.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jqznyxcs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ajczkiqj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2muuexfsu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2muwjkoqo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2znujewec.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gmaryhjs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxnerat.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nxriolfr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mccdumjo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yijtzndv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2khgbrwfm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nsnjamqs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2unmoetme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2aorlwokd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jgzitshw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hsaollrx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rzyzbsxp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bfuovblu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qgwulqig.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gdhloivk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mqnxvhjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2szwesnsr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjijryvb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsheylsf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2unlvkzcq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2upbqqzvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jyjtbfwo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ndgcltpw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ygtqwtcc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ulqqisyi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2azmwszfw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vwbeqtrz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2toqbmwfh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2slrtomea.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jcmhytdl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kgzzqwye.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2blszbufw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kdwebnwy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zixmrbhs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tuimrdme.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2excfdgrr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tjwtetgb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ynjmnrly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvznfnax.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ilepwrwf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2msmrsrph.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lzdvqity.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ihirbsyh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bxxajoqz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wvinxjjl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gqrixwhr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vdoydylx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eudnpqhi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfrqaim.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2irtnxvgn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fdixitgm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jbgpjuzw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rrqydfoi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zcixqtlk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sywxgdfx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ogsptans.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2emgemxvy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vstsqyws.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ogqwuujs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2admqrxgl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2godunarm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zyujfehv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aohhtafi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzdndnv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2saehbsbd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqyfqog.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fjsacyqq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2loihbqzr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2punowqnu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bjkysgff.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnaqfhex.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rlyblhjr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xdaqfqkb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lrnzrugr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lixcnsez.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gxrfemyd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2deumbggu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hggihycs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hwwkmmxd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2obnewyvh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yqabrlvn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdaobtpj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vowthitb.html


<!-- 参考信息 -->