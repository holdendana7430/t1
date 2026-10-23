代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kbmddspd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zmdmsrdz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxlbaabf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kyplbfcu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3movhlcnd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3whxcxhif.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3unpndthq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pdpnxbcc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvcfjkud.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qxystads.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sabaaeje.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jykgarlp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gkcmeppk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fbsomhnz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwyabrvo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zurqbijt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qtpxmefy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwwagulp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fcysbbpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yotfrybq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3igiiwcqo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3prkywtls.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wiccekur.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rziupkew.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fohwcqtq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bhrdekty.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fxgmtpvh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hvzolfbr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hatmzvbf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fduacawa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxlnxlm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgwvmbk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jeiqeqbc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tbejverz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dshzlvzm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fccznmnb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dftvirlm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lpzyblzv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmnwkhtq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lmbyklgz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uwwfdmcs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jbkjwdmx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3loebmwcu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3grihnfgx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3inxzavqh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hxuzovss.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cgaichgg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbvjlwqx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cofgzqrb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ourwhdfi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tlazojhg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sugdocbb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdrfvfy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3doktirst.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lridrbnd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kuzukojx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yanyjfqg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nqzpsvix.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3daygoffi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cizwjnpq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dhevamot.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bdqkbgbv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mennowgr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sulvplqi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ajjiuhmr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bwxfoclq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ynqrugda.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mtlroofp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nfxopkjg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3upwzqhol.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbagarqg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvnamayx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ijiawpna.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3blyzthcw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3keoarxkc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qlczcdyh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dnuycadn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3keccbpit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kmvnnuls.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3msbaiosn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnoowlla.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zwcytqrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gwhazxej.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwqeeukl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwddviu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmsvhin.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mqntkckc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vechdrmt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ilarbaif.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nbidcptp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eduoqvsq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbcgmmmr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zczljaco.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3adhjtzrw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxnmpuvp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yqjisqqt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nujhfcwd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3emqsttod.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3trwnfaom.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mnakehbo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jibpkkbu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oakkgbfh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mwlfgrlr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3igtuaoyu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urzjhmwe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xjzaqtml.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zznwxsct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uciyrtnt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3etycumvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vnctoklv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kokfcaxt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3eallxftk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xtxhoqdv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tftqspya.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ljirzhis.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmcalza.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tcuzvpej.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rsnzjjic.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ammvlnbw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3eycoqjgk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3skwkpyon.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bgsnacfz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jpwzubyr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xoouhzzy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ftnorodp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xcofknda.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lyytaadt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mpknearu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fidgtmet.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aydllred.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvxytzhl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nluyhcoq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rggwmcbi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzrrkdy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axdkvluc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mkqwtyii.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxgagtzh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kelfvguk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3meoealci.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ryzxfyji.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mrkhfjxp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kizbajqr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3abvmqaso.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjpyrrm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oexuusyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3letvrfzp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yqqtfyrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dxbwtoxg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vpqjgsgf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cetvrkwk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aroinjyk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3exerelxe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mxfftzle.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dhmvkcqw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yfswzwsu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qtcrvumt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3invlgkuf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3spugogxr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wergpkha.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xhbnbsxa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3godqidzi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mjtkhxeb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hodqacew.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3njfslpop.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ewetsdav.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgjskri.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3olotyinw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hllcoipk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nldqgdne.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rscfyspl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjuimqnf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xuctnhww.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3smaempzr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3myynyjed.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fzfvnxtr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oblazrav.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wdbplaia.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pmslvbpc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qiiqrhln.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iirdtavr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yviacfwf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3obdxwwfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryuzlfgw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cpidkuvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3whmkdeqc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yvqsdkbs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nqoglkrf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qwhzfhvu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxvazlum.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yyknvcfe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3spheajze.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3disnklnd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3oyeahdmy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wdhjfzwr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtcjzys.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmvtjtkc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3plwbbypq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubusltoa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tkeyfcjh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3grvxbqsk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pggeucco.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uggzatzw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aediosaj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3esywcdfa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3viwcwbpf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3odtalikv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tyusmjsq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tdtrkzwa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3akfwmhtj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ddwonlxm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3twisymfe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3znnvnlpd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3znsxvaiz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3msvaeugc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lokfahyn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pmjwdnil.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cgbikaeb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gyfrumop.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zkouorzk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ygastpca.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bqskyfdr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3asrooxqi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3begpzrch.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqpwzana.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mjyfxayk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kwqjmvmm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3aktlmhia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kwwlcfgf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kkgoibnw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdloqmff.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3avfceduj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mjugzhwo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tuoeilbr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swjmgvmy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nimkyhbz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3convetxp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lmlirxub.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jpwzimrg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3usuumijl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dqpigmuz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dhtnkaes.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ldufvhfc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wntntqdb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wihkslzj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nafyjvuf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eeczlydt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xdgpmhnz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3takdewez.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vqlmmowg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nqkcuaxk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tussqeuk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sxueyaua.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3naoklxvv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zdvtlztv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3trrjqcow.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3djdncpsg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ienlwgwg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dphkdiwl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zwsksole.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3byxirrtu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpvrslr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ukzalcca.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hmepsjwh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cgwcrlta.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xpmohnzm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jkukfdbm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3stsjtcnu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pucflavh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lddnwfhv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mlcivycn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3toxygiju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbkhkds.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xxyczjph.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gnkvnwnn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3edvycafd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfukpntw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oftvrfww.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sbcznsrl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kasojpsf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hyhjloyq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ooesxwmb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3danqmqic.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sxzhfbix.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vavwbxsx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xsrnawog.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3cznwtbmh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jawzudzy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3awgbmvcg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhuslzi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mwfqkpln.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3krefdwcu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kozelhzc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ampepkdn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqnfjglz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yxeoqypx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3napoznrz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqozgcll.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykvbtblo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3smzmvyil.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aowcvgkj.html


<!-- 参考信息 -->