代发 wailian999

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gisqltvzg.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gxaiwicat.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gogyehwil.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gcfrmzpwi.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/goidoayer.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/glfymafrp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gsmgwyjca.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/grpywejmg.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gemjpxlge.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gsodmyesz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gxgqbmnwr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gujiqfujz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gxzfwpves.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/goatihlwp.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gxpniulda.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gitttsbsq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grjgdtuub.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gywekeifd.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gkoofippo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gypoxutih.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/glmgzpgyg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gdffviixs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gqupqsqzi.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gozzwuuwh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gvyyekxpw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfzhomfll.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gqnwhgqlt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/grnydkozh.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gaaicpbax.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gefnmqvga.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gwwuaqvtb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gywmxwxgk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gtvyhlahn.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grwsuhslc.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gbmezllho.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gczaopzgf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gcsitfniz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gukisvkdl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gtvbijwas.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ganavnhfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/ggikonkws.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/geeheapqz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/ghwhxagzo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gqvtbnklv.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gaiefzmnx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gfjzjrrrr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giekopsmg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gyjgjtkij.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gbzsbkndd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzmaildvv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gmuuwogff.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/guybnxbir.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gkuxkdplb.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gvfspvxvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ghdhbwbiu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gwmbxqwhd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/galdbwcsb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggtjvijpd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gxqsmeugc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxsgtjqmx.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gvffqvzal.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gfocglcgy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gilevblgu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzbrokuxw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gleltbfll.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gocctfczp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gjoogzefr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gehdmqpef.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gyclbvzvb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gjzmaymlc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghjylzphd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gdivgnnvw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gruwybazm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gydhuwgyj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gekymmpps.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gstxgiyyl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfmlzvcuo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gkgnxmpjd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gkrwjuhmw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gpqqsmltf.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gaxeakltg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpzrwttne.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/ghuglokcn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gimyfqpvr.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvtvbdcjb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gwsuyhezt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gjbpsgiqc.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gilwoyilt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpdvtqmtq.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gxufaorze.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/glymvlqtu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfjhjdmsy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmpuuiptw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gafvevnna.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/glzyjwgdr.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/giyugfzsu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gnrclkyoo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gvjdacdyn.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gcxbhirqg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ghykfirjw.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gnfqjxjsd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gakwrujca.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gbwepgnkw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gzswlzqae.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gwhzebobb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gdbfpnhcn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/ggmylmron.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gfyxfsqps.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gvydepngp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gsurgkydr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gfipgdnlz.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gxetzryhz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gbjrixwqo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gzppbnjoo.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gnrwpftbn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gvtdvlnoa.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/ggihltrms.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gisqhoshh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gxxujiycg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gvldefaer.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gyjlcgjvq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gxihglcnp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/galvzwylb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gjmurpdcy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/giueaplyb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/guljwsith.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gffifmqmh.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gosfvdzsn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gsgkgxpov.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gfydwguoj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gymfczlnb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/glvubllgq.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gpkmayxgh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/geqroavze.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/glcenyczy.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gqgqyadit.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gjucyuqeg.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzsgalqdh.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/giribjbtr.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkkntbrkc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwtlmgzvd.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gpfouebmq.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gmnrzmrwr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gkhaficfa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gswugdigc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gozkklylr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/goowespqe.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gdvwkewcn.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gdmyddpxo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxkagainw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gdfmpfcxt.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/ghzstrerz.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gsjpgssfz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gbamedarh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gspkhzkxn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gpgmoyjfv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gnkptuxad.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gdhvjnrrk.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gvktdmusy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gmynyawru.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gbpjtjrji.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gcnftfbnz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gousbwlox.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gnxfxaqsb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gldqgzkgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfnwrsunt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gapvvqhyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/grukalsdg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gjnigkdvr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/guzrggbxo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gpfbprkdq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/geghodoee.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/guleqmbiz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gqkvpkork.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gszvohpug.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gyjtoinvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/geumgoloh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gxsshatnh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gdauyydcz.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtmoanyvn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/guaytezhs.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gnfqemfvu.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ghvradmqr.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gbuxvzowk.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gqoclqtzr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gzimbvwdn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxgttorsy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gwszfjicb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gigspwvjk.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gdmkibone.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjdvphylv.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdkmsorgd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gdgulclfs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gvwvnkzor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/guxsanlyj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gwvkrvpxb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gxwwjlowb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ggchipxkf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gkqeybxdb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gpwctvaeg.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gncuzkxzm.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gftdvtjpv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gthdkjqax.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghnjevmvi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ggeivhsnj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gvjzwrnzr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gfzbvktyk.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gkhnjvrhz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gzolvsgrw.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gwszglhyo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/grlyoyigy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gxttgfcqu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghxyiqycs.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gpqrusmwq.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnykjfnsn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gomlnehcv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gdnppdsop.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gqsljusrp.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/ghngjouaq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gicacrvpu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/ghfltmsfa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gjmquswwu.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnqsmfpiv.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqqpvumxr.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gbczbdntv.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gojlcplxs.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzauowgip.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gtlvhwfpv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gezegvhxh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gavnjrtth.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxavocasu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsxfpqinm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvmyjhebx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gknewhuws.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gjxwgijci.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gfywqxmqm.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gmvmzdvtv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gcbbdglng.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gopxcxcsp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmyicotld.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gyrqufwar.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gecanednj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwmrxvrel.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/guuzrnkax.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gudaybdld.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gvecyjbbj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gxcafuajw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/goezdrnxh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/ghrudthyy.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjknuhdsw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gbjzjqcqf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gdbuglzow.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gugpusagj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gsenrqzqd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gazfqsqhi.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gbguqemnf.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gricdofcm.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grvurusek.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gyevabhwf.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdriruqai.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gxqkukpmw.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ggkkwqlfa.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/giqvrhdfv.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gzqqujasw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gwzhjvetu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/giekygfaw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjxcsexvv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gjmtxansa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/goplqdgad.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gzbagkpxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/ghtozomjj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ggjaqdtcs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ggtmljfkl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gonbvbkpw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/guxjamfiz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqqknpron.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqhryhosa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gdmfosrfn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gvaujhuvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtbxmtvwo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/grhkqnlid.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gayozuylf.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/geuuegwnh.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gduicmiui.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxahcafaa.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfszthzck.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gksoqbvpy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gyjiqifek.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gensikzoh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gdlyueueg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gtendrgud.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gjrkjqgqz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gdtldfqrb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gnbtcazji.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gtvddxojb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gdegceojn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gyccpqpqw.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gipdktjqk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gygbvkvie.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gcuxsrolq.sHtML


<!-- 参考信息 -->