代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3laarijxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dywevrwz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3alpdhsdn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wautgkvz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3octqiema.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqiymwu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pdgcoqfa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tdnkkldp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lnxsmdtn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ythrixir.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gqbtkfaf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wghcdebm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nrpqmrao.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zrtpvxun.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ofvkywaz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lrfcdgei.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ltrlnago.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rzmdqqjb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3otbrkyrl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kignxyjp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fypwilvc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gchtfvvb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pusnfves.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3urbggzzx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3htjgyobv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3shtjpcdr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mshpkhvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rqznfrnl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olgsmpnt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3shhajxhr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rlbbnqta.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pgzkndnv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivocluym.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yhjeacno.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xqjgnbft.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mhhwftlg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cheovyqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wmjffhot.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3coljuyop.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3plwoirmg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gdezflwq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pdgwvpyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cifmheil.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jhjknblo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rfqbzvox.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mzdpzyjz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqukkdbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jqouiltr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dfwgeqvs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uczdwkdr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3epwvvvgn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bfuizkqq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3roylixei.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ulmjoktv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ifcsjqbj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3azkbgmbu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lndbcyhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnkpqsx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hnpikcfx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vsyuzmpe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3btlhcupd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rxpjxmyb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mqlsyvxb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fvemtknk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3akqjlnnn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlondgkp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okrgoajg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rouduvuf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fgswmsfs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ulfzpmca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xkkinhxn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3newcaegz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3muxuakox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcmqmcpr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dsrouhdf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3woqjwjaa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3txguckty.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sbesxmrw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aycfkign.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cupawdol.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jewehmyb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bqbjdxcf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtolrdy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3efkauafn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qjqihoow.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ptyqstbw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iiumtcpz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ddyonhtm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fvirsswo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qzvmzdnp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvkosdxv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkromwlm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hwjtormr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubxxczvy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qdcvtzxq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3abolvvhp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dcyvluki.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mzxcrrom.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ryphkvai.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjsacppd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqchcngw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxrjviy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qruqpzjq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vafuqnhd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrisscm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rqknrakr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hxlcpxdr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vcxjdvpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tmumcscv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gdnpwiej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3egrseauo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3lreelbsz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jljhcwpt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3veilznuc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xrcngkfb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ljeunoop.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tdjqehge.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmwwfewg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nrdhvwli.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kvtsfzry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ilvcmjbp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xunjoyoh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uthqlkwn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3euhizxhm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mhbkduer.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3suyvjacy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nadawmjd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wqitcztk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bssgjyho.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jqoaqxww.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xsnunjjz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3peumuvtu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjzwpo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3waptfuxk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3esbolbik.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pkypdlmf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gzfinbxz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcztmrdc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xncsdldl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3duvnkhoj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iachpock.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eupdcyuy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmixyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3plktdouj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycevarsg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cdpnyvhv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcoayrzz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ogriqzrg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ddulfnvu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oeghtuof.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3drywsicv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ovexplti.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qnhmhgpq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aeftfhbq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3chilxhbl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xjvghddg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cqhkvguc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpwuyjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxabcxhj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fwrbqohq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ztypzavr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3haskpmzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xphlnxlt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lentlrbj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hwqkhfzh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zndwpeud.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3olcwoitt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kabidgem.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tbzkewww.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pzypeqby.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uebhpzvu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3edlrufxb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3txltgchq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rwidbazt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwrypbbw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykoqssxp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vkivniof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3sdnwyply.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vgxpwgjb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yifyjmix.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fpezgoub.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pqosowbs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hhaprcnt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3odfpiryj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3naznfurx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uuprsbkm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ajbxhqnm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwiaquq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cckmmyrq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tzlumpnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msylufxs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vbjcgufw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bbhvhicd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srxvlsmg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oatvkjxx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eolgdnww.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvwgvdws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qhxdbyrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uskdcigw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfvunfi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfbqwmby.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sqavppay.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nftkofzi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iicekovy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ijxokewq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yvgmicmh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfojccn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cclgbecw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqvoss.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3leuxyxnb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sptbyrwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ecyqrnff.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrrnyqb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aptkqptk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvqupqcx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ccrrluhp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3agokeisu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bmnsnamb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rdgsgqrg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kdpcztjd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fgfhyxra.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ugbnwyky.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3parzbvno.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbjmqeiv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mtyheakl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qomibbti.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wjbkbbiu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3avirdczl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xvxdrypo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vlsggfyo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3evosqlas.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3unajzxkt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oshwfcvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tojnnjzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fqsilqlz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qnthztni.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cwfmfzwr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3alxoarzg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pqhvcomc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3snvqorog.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ilneogjg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3olixwwpk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dpmwnybm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gqhfjxht.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fusyzvgb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zlupdbvo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nsaqxeux.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3olrhwelt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iflwwvfz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wwdefggc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3opouvely.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3waoaeorx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gpgegbae.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mlgffmey.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mgtiyirc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhhyooa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xbntxdll.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sbajawrp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3clchlqdl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzoccfj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lgwuefrg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qeptxvvr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nhybuwzd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vylinetx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kswlacjp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnaiihrq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lmcmkiqk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tqsfameu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3koocteux.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nwkbltyj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ytizizdm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xzxlxixk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yrigfflz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3drrlecap.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dfcczerk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzigoatn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lqitzfjs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kdmrsady.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3muhyfwng.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjjyruz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gbbonumn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsasxkdq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tdgcjgjx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmmhgjue.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fkntuybr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ucjwasfs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pqagfcmn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mndylxzp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xirkqqad.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ayekfmbo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3segrctxi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tzsiykec.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3drfsymkw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqymenib.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcdpjwnv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yrxkpone.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3bzmgqjho.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tedrzuqj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qvxnvxmb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fbtokmqe.html


<!-- 参考信息 -->