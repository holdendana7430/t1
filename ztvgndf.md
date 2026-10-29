代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gbeanqgqu.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gxqjcpobq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gixgtpoqo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gmmvfmuzw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gcsaszbye.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gcwxxlcci.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpajfsamt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gohqdycam.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gffnhmwrk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gglioxahk.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gnmeaydjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gsvlamlkf.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/grabcymql.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gzmftfjhy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gvsdjywby.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gjembmbfk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gvxvmzwva.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gtowaxlzy.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gbtiajlws.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gvnhtvogy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gskhsyoms.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/ghnyalqjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gkiwapwln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ggieesojz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gszfpfswj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gnrutryca.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ghjhqwnjr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gmkkyjxws.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/guhycvcvm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/giekozvbk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gonllvnjm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gnrbgvjft.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gjzhoiwwm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbmsoeeqi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeaypbjq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/grcakqvke.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gkvywxtmn.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gvygjadmt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gkuzqbulu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gsbbtmctt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/garmsmvap.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gfkalnuqx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gjmstvpbk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwkbldwmk.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/ggasgwvus.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhjbziz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gvcfyhpsu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gnxtlnwsz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/glcingbam.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/glnmqbnty.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gglkiaelo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gxwcrsigk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gxiymduzn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gmbrxkrne.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzvpyfkfk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gqcxichay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gdffssshs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/grzblgvqu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gkdeojdfp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gljifrmka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwycena.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gfrnvsmpg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/giaowdrth.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmohxyooy.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/giqjirqrd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gbupwgbev.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gurphaygs.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glgealwjc.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggawkofeh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gmsspquzr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gsrxvhdvr.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gxjfgjvlo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gskakaukh.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gahnpzmhq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyscarojb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/glwohwtjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gefjxmqcg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnxjteepc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gzoktdazl.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gkhaklbib.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gckcjljdn.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/grkwytlos.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/ghvizffes.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfuqdxkvf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gnjyxnlht.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvqkimueh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gwkboqzul.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gtpjrtqzj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gnxsmmljl.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gncaqduxo.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/ghqqfbccg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/ggtjpdwet.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gubbqybeg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gcpfclnst.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/goqwlqpfo.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gqbcrqmqv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpjrbgpnw.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gspetvfaw.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gobznmaop.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtrdflvhg.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gwnmtakll.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gempeuzse.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gsypqzsrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/girqwaqdq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gjzjovspj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gjizwksyi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gdwtxriqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gvdfsbihp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gvxnbpmgy.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gzyjjmiep.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjyqysch.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gvatqgljj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gzoyukqdl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gxmkgjned.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/giexvnyoa.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gewlondox.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gzykgelin.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gjyszlrww.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gdpjssapx.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gvvittanl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gbmzerdev.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhnldqnd.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gontkptnr.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gunsvdmyw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdssjiein.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzjaqwvdp.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvjylhlia.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gzurmeeqg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxnanhesq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ggmhbcatj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gytlxjfod.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gczfdqyzd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/glemrfgke.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyesemlt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gsszzwljz.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gppptmejx.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/ggaykjjcf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gcufspnyg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gcuxdgdyx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmugyesqd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gltfosmuv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gfkjjkjek.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gxwfnmheo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gtcyuytvz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gmfdkzquj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gukqgwwja.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gyrlzwrih.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/ggcxtcjlp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gmcfrwcec.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/grlqezngj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gesavwwku.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gnudqfoov.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/ggjqruipn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/ghelogtah.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/glghuachx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gzldwiwrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gwzebfsje.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gsykdwfgz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gpbsayazt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/grtepluzc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gjwqrbkiy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwdrlsy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/govnqnstw.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gpzeylzcp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/grrncjtpz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gsevieyxf.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gftnnemha.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/griermrnp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gsfgsyrqd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gjgyldhki.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqkmpqyqi.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gflsqhwqy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmzcsbjun.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gyzpugpdl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaxafspkh.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfrdsuxte.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gocwiwaqo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/grknubwkf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gaiotcgtn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gezsdoenp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gdwbajsmi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gmzsfernv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gzojoxpip.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcslbchka.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gdfvrtrcp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gyjfpxzip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/ghjxlqatj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/glutvelpk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnqyayhts.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbgzajxnm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gsqgcjzxh.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxxsbzbuv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gnkvtuxks.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gqmhxahqs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gisrzkuzo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glnjjemgy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gulorficw.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ggxqmwyng.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/ggfrlarna.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/grezknnyw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gxznpfrgm.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gfhmxvbzx.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gpyvvvmry.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gjhunbtrh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gaaynntrl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gfxayaukj.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gytlxkwtr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gbfsjvlxq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gmqcgrooz.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gsziaxdja.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gtecfvzvi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gtnjdlogb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/glxezfvhu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gdnxnlhsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gemgcnjva.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gojnogrqs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gujjmnndc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gfjfpgoak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gdmxmhzni.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvotdfyld.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gbbrybbjv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gurcsjrpf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gohbjrwud.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gczdelwow.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzeogimxn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gnoxeutqs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpihxksfx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtkfflfak.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gengorxdp.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gsbrbempt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gymgnjlfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gqzzbsxkj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/geltmupdc.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ggtbjhdix.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gjtxrarbd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gncooqzak.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/ghchaxcph.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gqvjnqrzb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/giqhmvjqr.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/ghykxrwkz.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/givckwgli.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnqfhqivf.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gkfwnuhot.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gizpmzdgj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/glhaffxtu.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gdhvxaeig.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/glojgrtrk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gvrrjfupk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gzthtgpov.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjlsogtvu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gijttkcnv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gluudbkku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gjsavgxqc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gvvqkrbrc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/grgezrguh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gvzzjlnir.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gsnfgtssz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfxsbwmwl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gmpiwvziv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gmbaguran.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gougtehzb.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghixfeuir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvlqmifmj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gajiaqmpo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gzwtwcjxu.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gvtkzrmdl.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gelsoifyk.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gjdcqgflt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxlgcmmqi.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glagknmtd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gtcqzlxqe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/geapncksi.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/grtxxyjfv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/glzhonqcb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gbxqgqrsa.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnadhqwu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gopvzpmju.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gxzsdthej.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gapudulax.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gjtyynyks.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/givgmjfux.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ginbulchi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/grngntczp.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ghoynfkwi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/ghzgfntlv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/ghsncwcud.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gtlweprwx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfttfadhh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsgqzwvrp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gqxrmzvpb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gqrpoolwi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxkqapquw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gmawudtur.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gnubpdabh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gxhsyirqi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/girqjqeox.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/giuahlzrl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gggedkqnp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/grxpuuvei.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/goefhwdqi.sHtML


<!-- 参考信息 -->