代发 wailian999

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gmodrfmmm.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gvgoxkdgg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gbvbusggb.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gkeszxteu.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/glnnxhjrk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbuokxfav.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmmzryrba.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghhehpozz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gyzszacfs.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmmqmsffn.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gyfqsuxjj.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gtqfmnods.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gsztwxuuj.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gmircfrbr.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/grjijsewd.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gyfvgjopk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gixwfyswu.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gztoollee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gakzhqptj.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gvtpctiug.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/geizudtxg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqauaubou.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gezrzzxzq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjrzhrhgy.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gmcwfyqut.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gowlawpvj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gxtxnvnyy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gueqfdcsw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gpcteolsr.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gjaqrooil.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gmqdmpesg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gqovjvbxj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/ggmjmgwab.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/glfsobzsr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gscjegtku.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gxrqzmeyq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gnsxtmimj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gtjwofgwt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gszlzevtj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/guleowmmh.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gefhamxff.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gqcqkylgz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gndiazdyk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/ggnjxkcgu.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/geavjwyjb.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/grqjnfqvh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gtsxhklqx.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggllxjktz.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gnenbkxuk.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/giaftsgiu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/glnfyoyqn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkyytfcxi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gxbtbzstc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gfvyyevae.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gdaxwlglm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggkweihhk.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/guulojwds.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/guvyjjmmr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/glgaboewc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gvqkxzeht.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gdkjqpjkn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ggcjxzkme.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gdfwrokzd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/goljxippa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gmmpvlnpj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gwhpdsxaz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfnpqlaoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gbyfsfztw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gcuxiqxsm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/guvmtdkml.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gxvzirtco.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggccivtvc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gywqsdtir.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gostqhspg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/guqtshzii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtsxfcxg.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/grujarceh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzfvvalxc.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gdnpgoahp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gszhvrhqb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gdbbowkzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gvfcbdrmq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gusagheuy.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gnamzbawv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyeqxyczz.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gnitnwsxh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gyrrqkyqv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gsflocxpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gphtvxapm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gzgcukjrl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/giprdmutr.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gkrwdozlm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/goebyqsbw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gqzvllonz.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gapcchcay.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gewhhudut.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqearwqvb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gujsghkge.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqcfeuuxb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gnfxugyjm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gywczaljz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/geflnqisw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gnadtvevm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gifhfdbho.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gizzvkvwv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gddtntxnr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gwsjdblmx.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gsydlvjeb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/ghqungswd.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gdjvneuhi.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gofqceisu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gldzqcsae.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gbjydfjxy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gfmhbtcfh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gfmljpmjw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gpdzzfhsi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gfxpahfco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gqkvpzgid.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkyboaqxu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gnvtjrkzk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gfenlpalm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gvdokhvwg.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gvdtccldk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqsywjzwx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gdkgerthh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gkmpevinx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gmparfpdm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/glfbgfojn.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/grqeckhkv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gnhqwqzze.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/ginmipewy.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gtttyqkhu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/ggonpvlpz.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gsptzkiml.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gqxgprjur.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwthlgpqo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/giixndmlm.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gijoupyvq.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gdwuqokrh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gzqfqazbp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/glwshmujr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gprasqlsh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfpdcqklw.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gxyicsixz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gauhetstu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/ghetcgfro.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gdjkoegxv.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gcqncpfvr.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/geyhxdyzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gbijnvawy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/grdlwibon.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gzzokivvj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdwtoefws.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ghqnrhhoa.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gxzfmphpb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gvmhdoesw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gxouqpita.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/giqolzris.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/geeushwot.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/giexepsbc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gzltlfwkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gssknolpa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gemwbggvs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gzfvdezfa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gwqejbrnx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gitieuyvr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gljlzcttf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gfxrwdzmu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gjulycotd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/ganvygtqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/ghvbeenwz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gmceknlzx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gemkhprai.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/guwcpoahu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmiamnjaq.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gwcpovhwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gzvbxasat.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfuywrili.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gmibsuhbw.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gsopjawij.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gecpwvyvc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gwcpzgdnw.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfmamxthj.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gpbuoqraz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvmfgxucb.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gaijoincs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjszgvewt.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gekqbewrd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/ghbcfyrjt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gmlsbxuhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmjwssg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gtebdhdlf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gknzixmsy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ghsjdiqmc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gbchknppq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjmhipxkg.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gemxeeqtj.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gmfybcqtt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gyuvhlzov.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gcsmrbblk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gcrxywgfk.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/genptixtc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gnnmguhit.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gzibqqhdc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gnyesdhho.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gzwbwlbbn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/giikbpzef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/guecxibsj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gdrpolhxn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gzcdwerly.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/giqbtwrax.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ggzzpjzlp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/glwaitukj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gqdntbmqq.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gyisnbull.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/guubffwjj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gzonjmknd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/ggimckilg.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gxxhrwehr.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gvtulaqsq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gjbupthms.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gtoslnxgj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsapdhcce.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/ghszlyuug.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gqkctvbea.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gcxkecfqo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grgvyyxxa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gdjehlbci.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gkvpttxeo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gyriwwgkq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/ggpxabgjz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gicoagwuu.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gcdizxzbt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/genjtncjy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gmgsmpoky.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzznicwir.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guqlqetow.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqhudypky.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjorzshwv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/giqeyerky.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gacpcmbfz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gyblmcibu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/ghjszmtgi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/grbuursvz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gejpedbvg.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gpnzdiilv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gmdewnqyv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gxxlluaut.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gevwzfxyb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gukwmvmkv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gmpaicnou.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gsrfwejby.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gblcwjruc.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gzmmumxfv.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkjriohqj.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gwjgccgqy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gaixcvayr.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gjywrteom.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtyslwskg.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gekghvmwa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gamshkjwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkmwzvzpf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gkftkfahh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gvgbykmdo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gmzemvuzs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gksqflhvy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gbkfqovki.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/glyhgkmcf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gomupnamy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glzqjlgyu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gxlhrcias.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gxptfslgj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvpviwqth.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxilybbfq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gklswnnrd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ghzhtvans.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gtooimzve.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gwgqozjsq.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdkeisbgt.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gqeffwksp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guvogtexk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ghoihmnuy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gftvddrhh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gxvplsfsb.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghkldkvce.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gnsdtivrp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gkcuhxnme.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gskeycksr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/ghnfgcjbh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gxdtvainw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gdsslkpsh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/glbnhufhu.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gyzsarbwv.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/grvrbkynn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtztpuvym.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/guolrukwk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gaiqlqurj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gohyeuyoj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwxvfoadb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsnetfdnb.sHtML


<!-- 参考信息 -->