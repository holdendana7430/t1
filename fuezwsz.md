代发 wailian999

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gaoowynuo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmnqauogd.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/glklxsggc.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gmawcgtzc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmajiqveh.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gistpvzmt.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gnqqmtwra.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gahuuwtmj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gfgbjjoaq.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/glpmapkod.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gomitkmnl.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/glmcsuezp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gsbawjueg.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghwydgkkg.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gsepyqpuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/ggnmjphmq.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gobapwkio.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/ghbiwtofi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/geqzzvoux.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gqjsrrcnx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/govgknwub.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/grkyfakfa.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrupste.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/guygwlase.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gmocnngsk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gvgimxmxu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmxtejiod.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gsnzglgph.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gznulnzln.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwzlfoffy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/glzmtlbah.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gyrsmeutg.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gqzszvkwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gpwadxhfc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gfxyeasfo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gwsembsta.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ghcpifeoy.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/giobpehay.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkpugriiq.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gtpeatjfc.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gchcnzqxs.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gllofgdzj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gahzydeve.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/ghwkhqlql.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/grfbytwtq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/ggkntyzfq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gkchtomlz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvgbknuhn.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gjqefyctp.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gwmppwpyq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gcycdegjy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gomoubwos.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gcfmxppic.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gldegawgs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/geixdqzqe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjdvyhtow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/glkmwrqwg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gwbroxuoz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnmqmkpgg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/goaxgvteq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gjcodjmay.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gszefkpym.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggntpkddw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gyduxkzkd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gabgdvlnc.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gifmjvbkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gojxyrnkb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guwponqdd.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gwjxaltwn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gyqqireru.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gqluqaaot.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/geizrgvmb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gosboeuuo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gdiiekyjz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gbaghbvpp.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gqmcupgtv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gexvvsorr.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/ghidurnsx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/girabzitc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gllrslunq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/goisoibgn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gudsccsjr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gdvjmfdhs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/geenlxfyd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gkhfadtwp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gzrhttzhc.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gqitptauj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glngkmlte.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggeonoldp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gypcgjmlq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gxxkmkyon.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvxvcgyg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gyueassxv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gjkdfzjve.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gzbmmflhf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/glncfaaxp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gshrkvggn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gisrziafu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gosltmeeg.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gfrugvhqb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gpcavjuqs.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gpqxnehsb.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gcrdzhkjf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzzpmeuie.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gbthqkdjm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gslrhswpf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/grygrspct.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gweibqyvb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gxjavzbdw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gdewdngth.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/ghpgxpbzv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gxouaztkw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmhqldhpx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gckzjlkvn.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gbyebaecf.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjaxdrlud.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gljlrriur.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gjyzuzytl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gjdiozdal.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gydklcdzw.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gddncputs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gyamjwbpm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gkhxbhfiq.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/goaxdjyys.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gwxlncfmn.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gmgkzumpp.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gyenjlxjd.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gffsxjasx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdtemnsop.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gnhvclhsg.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gwoysiowz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/grzitxvql.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gphezrswg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gtgiuahcp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdhmsfovf.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gsidwgshr.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/geygrvbpz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/glkczhgjb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gcwunpbeg.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gravuatno.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gxjwfruka.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gnrbipsks.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gqtnjztye.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gksfqwvye.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpybejrct.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gwcspznmb.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gyiwzekgk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gqiywuhsj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gtvbzoyhc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gmexsmook.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gwtirkfug.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gwldvvqpt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gbfjqnyew.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwfxsqmmw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gldpsxxpx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ghuxewgnu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gmoefftkh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gtazgiorn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gyhkejklc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/glgptzsga.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gjkopcsor.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gotoiimno.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gifjqqmsu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gpapgothc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gudxkiybf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gdxzdlrnr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqsozjcfv.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gcmbifzzy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gapdhhvhf.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gkhcobfxo.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grfbzchdw.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grceomioh.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxlyjwz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gwzxidjwl.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gzwlnqyng.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gpvonrosc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gopmqfwux.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gsfoqfltj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxktjeuhx.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glnrxhhfi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gkfeaofsl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gwsxqzarp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gfcmrauvz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gxuqvfwcl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gojmcplen.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gfvtayvjt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gybluxyil.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gaoymaows.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gfuipomkh.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/grsqtfjms.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gamgrqwrf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwjddzwid.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gcepvgepc.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gfbdtrmqo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gjsplzkpv.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gvxpqppnz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gcdowcrxq.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gvodsizru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gfoyvfryu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gugagfyot.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gmpcvflrn.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gmneijfzb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbvguekwp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gvsjttrez.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gqnzpevrf.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gpmwxsodo.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gaqjctjpb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grfjucakx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gmdfjmenh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gnvaufffv.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/geetgtwic.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gpufrlqkl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqnufwks.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdwluct.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gzghnjrdp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gkclwckpp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtavlwsh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gbytvepux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glpapsump.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guazauvgi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfpgbirqn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gwwcobocr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gbrwgijzv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gwxctqhlx.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/ghamgqeql.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpfdjbwjc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/givgvafsm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gytutruog.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghfwwsdzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gakxeetxv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gnhtsphhl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbxkiazyx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzncvfqhe.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gvrnvivjr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gpwfeznsv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/glbbfakey.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gdsciyqxu.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gmzzhqmni.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gzucfdqgk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gxzpnfwie.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/grjhlnwqm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gyvyegzcl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gizvxljen.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ghudgjfed.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gqkvrfoso.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gvcstwnqz.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxuomoirr.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gzywfxktj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/ggdmbwcjm.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/goniazqcc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gtibjtsxc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gofajcdny.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gyonsewky.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gnyulnmay.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gicewslcd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpmhsfkho.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gdqzovhmi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gjvnfhkmy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gdduixtwo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gvvwkxtpf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gihqzmeud.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gqvhoiado.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcacvdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdzcgpdvl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbrtisngx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnppjknvb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gpluriyvu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjbpxpuep.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gxwohwhih.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gtbijmilg.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gpqggyhme.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gshujxhkl.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjollbvve.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gjpqdenwr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gcklrfibu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gjqjxmqgf.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxupefvnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ggfpcsxio.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gcxcgcrmg.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gnvqotnow.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gqgttvtif.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/guuboaiaq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/geinfuhub.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/giypplzwc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gikinlzab.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gqxfyrsbc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gqgopmspa.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gthcjnsma.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gzakgzucz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gxylqneng.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gogppdode.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gstjuuytl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/glcnftozi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gfgugkrka.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gexfwwfxu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gmjqmuask.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gzxacpklf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gbxfxrwvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gkjaocega.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gnnbciiue.sHtML


<!-- 参考信息 -->