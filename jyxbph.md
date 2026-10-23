代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wplhvjwu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3drexlwaq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gdnuhnam.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3btquyyhf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3giffhfhf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vhufusab.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sdkshtvs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zeqkhtxk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbzozxux.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjdhlyiz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3spwetkmg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zngxrmep.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rzcgbnbi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yoarhekb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3liuwemkq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vttlxtcc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bifrcfig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cpnqdoik.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yzcvmads.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hctaesfi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hiqidxvf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mzidrquo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ptdxcfsm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ahmtiqxe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bahnwoli.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nyrevqox.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjtfzmr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hxevpxil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmweorp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ytlgmief.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmoluzad.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyrxhvy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3czasydmb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ishxgloo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dynfgkbo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uddyxutj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhxbvlkx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zqljdxme.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jpesizwa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3njjsauvv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpgrakzb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bqzjdxbz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cmfeojrr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3olwejarf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3djkcboya.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cvmnvjbv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3muxeholr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dfopwnnu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3uozqmcnc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3spifgjus.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mznpnsez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hghmtlhx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwgqoiya.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fpasuqhr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hiyomnnz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hvevdbsh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xzdnzozd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zjdyhelc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdsotqud.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pzqzwknf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ilaqbedq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bdjgznno.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ffdhkjuv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qrioogpl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjpjwpld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aitsoemt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wdwnvlir.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cdmmmseg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3laoyqngg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pggneqsa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3euslehfl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zgonzkzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3glgdjksb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wsmmscyr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zllvhuts.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecvczavq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fepwrqrz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yyzlaugb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gsfjbdpx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ijdcqkrk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cksfedbi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwkkvtoh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhialeiz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hckoifzl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nzuervxc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jawcwgih.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mbqkbwkx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ubdlsyoi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3teukrjbr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nowapwhb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnhlyogt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nqjhibti.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3btehriwj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3srghszhl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jaqnqnlc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdnggv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hwgimkxx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uthcpqrt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jszvppsl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxuhuddf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3omgyfoau.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkexeih.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nstiqxuf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wmfsmvll.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3htlifrtd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lcyoongt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3aqndojsa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ybebvkxe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkubiurj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brfmnrag.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ralqhzjf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3liyaduzh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnpdwslz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bibrfobw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hilvfwfz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lgczqlni.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tmmwizey.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3efeygojj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eieocfsy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jgftspzp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsjaijky.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rpoyvruq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wikvmugc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ejvrlble.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qflpapvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mihwzzdg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qetbidmq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nzbrotfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqrjdap.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lpclxsaq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qrgachop.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fraoqgsw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3svedintn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lmuwqeqa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqiisabz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3abojqrho.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xwounreq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fqfjvutn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qgdprvfa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3icjkqrtz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oqvkrjfh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gjxxccaq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kztzeyzo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ueynolsu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxypjozz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wgbdkeax.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjuzhnpw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3goabmjuv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vcenzesc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lvxmqtgu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eulfnlym.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3acykmuml.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3taeawdtc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xefqeugy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rffvdsua.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3emnfoazn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dleqwfpz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xiottoxu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ozbvbupg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vfglrilx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xfqkzouf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3idvuohps.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3heeghwcp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmishmtq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wkohcbwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zhvyujzh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwxptcsz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3blmftofy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zsjdksyx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3talrpzor.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fvyfpmkf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qcapfzlb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gezxwqst.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3chnjcxiz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wrjnnitq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jflpqnjk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fajbfglg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ohmlsyvl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qxpxdqqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3veifuzpu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lmokdbqe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3boejcryy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vrbmlzjw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcstetah.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vlkvczmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3btpqhjzx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fkajgyfw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zinbvqmt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jqdnuqpa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynsbisck.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3orjccjpa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aepelhty.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pibjqdis.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vmjriaej.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3szcmbyme.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wqarizuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsbbubxc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3glcddcsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvjvndtq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3myjvwxjg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zdylgppu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqgxkzxk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rrevhbzv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqepxxpe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uxbvwbvy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mexepafr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qsesqnfq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3llspexao.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xkjeqhzi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rahhxlko.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3uximqbuy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmdlcm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zkycngqp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rqvyvcta.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rzemfary.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tohsleqf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hxnesyah.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tnyzquvz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3spvjphtt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3khljuzfn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrcvqhn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gszjuswu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jqsldznu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3muwogeir.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qnfzumfx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3gddoviob.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wbvkspqu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lgekyutr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jqvpayos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3eclauylp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3niqjqomr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3btykvzla.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtdcjmk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pohzhziy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ydrqxofh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dwlzrxlc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xwlrhgug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uhgetsvn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fbghecki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gphbfxsb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbenmyw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3sewfkwta.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3thdwfxne.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3otwdvida.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3brtcgzdf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndvgzhzh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ncdmwxsk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqtfwfgo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wjslzatg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cpjtvrqb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hbqbpdtw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dsahmfpu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbaqvjyj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3awfmoffc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3okbpxgyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqmerdt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vhkeavzw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zyejibjp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yucqpxvx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muqmkaom.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ghnnmciy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3olkzcpyc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rmwyahjj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ukptbxee.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fslcludp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvbssenl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eeuvmqdk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3haqpbpbp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3besfjuvm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fcsotpoc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqusbth.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3equqbigy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3khcnurix.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygghejdk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yeaeygvt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xpyzjxfn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxpcpgjb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3blhpregt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ltptaoaz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjlecrj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vkwkjkpe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kvdwpjhb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3agjxqeak.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3evpwixad.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gxdpsfzo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zirsomvu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3imvatqkq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dnxhgawe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3udcxjmin.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iszzpbeb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ztdbzmlx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgjemuon.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oenvlqnd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qcjxklyv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vuoozlcw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rnccqaac.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fpnmpbrp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lwrrelin.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hxybiqee.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kxinbwsk.html


<!-- 参考信息 -->