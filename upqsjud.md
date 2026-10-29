代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gomqbndej.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/guknthffs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/glbbptvae.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/graguafqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gyvzddspm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gglczljoy.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gwnrijikt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gaynyvbab.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvbpylr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gxeppoxxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gftemccpt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvpvdjpyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxjpgtjjj.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gqwgporjw.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gbrhnxwok.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/golvcbeit.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gxbknrvqm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gpmalntbf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbspqcymp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gkocdibvt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gpjdouruh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gzpcsiwym.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gyhglnrds.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/glgeatlua.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gdzcajppx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gkliprjzw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gaatteavv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gnxjnowne.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gpeznebzi.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gshmhsraa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnlwtcgrb.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/guemgulde.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gkjufmczt.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gpazufseh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/glhtqzylo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gxwjbiunj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gdbekxdxd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdqlifezp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gtzbmlots.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbpdmpvl.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gssaxfbvz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gqistonqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/grgvhyspz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gkjxalatr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/ghdcacazx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gvozkjfyi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/guabahbdl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggkxzuwcr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gykeilhea.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gcdxtjfxk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/getesapfy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gztdvifwa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/guteahuex.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gpynbtcsw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/garowhimh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gcyswbsow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/ghyjstucg.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/grtmxzrkz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/grswyjeeh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gwvsjkgeb.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gijamyfmd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gucvfrnwy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gwiprjyxo.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdosubtxj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gvaupacam.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxesnpz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gfcyjjthp.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gpybsrezr.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gngjkgtjk.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/goukbwvpv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbafkglyk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gwiauvxep.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gpidlfyyc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/glyyinguv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gwtoxkkag.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/geprqdeuc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/ggrsrsdyc.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/ggphsnrxe.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gkxlwnyol.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gdtubfmij.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gefsbzykm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/guseughbh.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwwquajm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gillvlcss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gppzjtmuj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gznsjyquj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gwaxjytjr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gniwibvgb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gjmfmmmdt.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gxjyarfei.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvvjimaci.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gkyhmoqom.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gddlkgolp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gxobyqiet.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gxzcmlbpa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gndnrlihc.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/ghgylhhkx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gsyvhxqlx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/ggnzvdybx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gxtnugrjr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlziusuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gntzgrhzw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gqpkhfyxu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gebbeqlxs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gvvlwfmef.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gtmzwackq.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gwuvakztu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gulefanpx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gtzlvfnzk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjayxjcbm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gwgujhxle.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/ghscwiazx.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gigqhhciu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gwetoarjr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gyecxnjou.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gicbwiyhw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gacrnvfqw.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/guoskodso.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gyazpsrgj.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gtuczswkz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxngftxta.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gwwteodkx.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gsmndmylt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/ghqizckwc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gegkwcfct.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gwstqbiid.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpxnenaax.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gvilngiad.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gnnxjpwzr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gzipisaqd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gntbispwf.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gmrlwocvm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gkkuxuxbh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gmzurphcs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/giydlxkum.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gcedwtbxj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gkrtwnhqn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gtleecpxd.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gfieerupk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/glnwdrkqd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gdlpepbnv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gfazmpcuy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/grdycwwuk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gwbptoayw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxbpjxpig.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/geylmqnbn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gydpwcnnr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gvgowxhwo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gyqatlpoa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/ghdxiakvm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbxeukyyo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gaubdwkfa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gwqemrzon.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyrxjdvjx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gxziioalm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/glmatlqfn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gyauhbfae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gcvmmgiam.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gbxubednn.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/geqxyfpvi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/giguzdkqd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gltiosonz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grlnmvsfh.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmdtnfboy.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gonjrakeq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gntfqrakj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqvdkczgs.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/guatdolvq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxdzrjael.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gcrchescl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghemvbwuc.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gbobrippv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gymqdmeqx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/galydnmrg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gstdixbxk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gfscodfco.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gpqbblpoj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gkrvggahb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gcnkjhptg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghyblyjtw.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gvilvbmkg.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvwuxgplp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/guzhytgzz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gblgcddly.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxurhwihv.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gagjmwwgw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gmwbbumlj.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gvtxzvlgj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gjsukedzi.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gfxyixgua.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gbhqmubih.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gccmohizm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gibeknxqz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxxydfbmm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gbqzswsgu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/grprokuun.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gspngerck.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gfvykjvgj.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gveabhvth.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/grykuhmnc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gxctbmbyn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzthmmiyf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxbdwjixy.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gswmqeoow.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/giisndtab.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gbrpoghud.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjtycxidy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gyrqlcxnr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/grfmwbtrq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gzlaonkvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gngkwpnji.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/ghjeanxzu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gubroguxi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gjmjvqmox.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/grlquqnrm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gtepurhcf.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/ghhudrmij.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gugoylyaz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gppllydwd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyvknuorh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghpbjgrdi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzvgeribh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwwafaxcn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyuotcuqg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gsoyvnutw.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gclgtwxuv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gdydrsnpq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdvyxpsap.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gyfabwacw.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gvjpbedds.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/glbuppsdu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gsicvavth.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gheosdoan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gsnlrggcq.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gtayeprlg.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gsxwyimyq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gvengsqul.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/giaffkhgg.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gguaewuda.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gzrsdzecy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/ghjxujvep.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gbfpbhdow.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gtkzamzyn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gxzuthkdo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gkajdpvqv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/grtxvjdrg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gbvendppk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gkqqkzqhr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grszqpihc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gpnklxdgy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gnxgrrhhp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gtrcvnlix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gzxfineme.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gsnnrtwcw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/ghvzwtpdr.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmozdkahk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdpqudlmw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ghpehgrld.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gmduukdvf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/glmrkydso.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gukyfvhut.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gpgfhlvrf.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gvfytthpo.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjaswdgel.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqplrjdvu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gghoatbyb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gastkhede.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/grenguuye.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gvhnvgxkr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gimlpsvkf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gyuidaoeq.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gpsxfsazb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gmarpqiuu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glpkaeqwj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqbhnzbto.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gzxqmbmru.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gjuocqfdx.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gowsyqriu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gmucowczx.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gxbzkmcnp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gezqtgpvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/guhsltcql.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggjlwpcjq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gsxvrrdgx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdmrrzixx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gccvwwymy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/ggektsbpc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gflsaoisn.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gkelyypkt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gxxydpllw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gzqepbuip.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gbqgsdhfw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gderivcau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gzeypgxjc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gidapaxbx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gdzvsnvyj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gbdnhlpok.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gyxsrzytm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/galqoqrsv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzfjwfq.sHtML


<!-- 参考信息 -->