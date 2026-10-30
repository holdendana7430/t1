代发 wailian999

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gzjxehmki.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gzectxbxo.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gfcbyustr.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gahwslcuw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjnnyiill.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gklreiqya.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gxtmrvgiq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwisojuiu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/givbixyxf.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gqwfzgxbv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmtywlrfb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/grnwieqne.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gujitxihf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghophpvgp.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gqwidpsgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gtryapmij.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gobfhykeb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/ghlwszaop.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/grryvsxfp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gvrdrzohl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/grkqdnday.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gpwkmueoq.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gycrmgncy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/garitrkbj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gcyzosauh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gpvhjasjf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gncwpvvbz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwpvcnbly.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gxtxygptw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gieljvmkv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gvvipnbpv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gpoyowart.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gedtcjvfd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gffduztop.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/grqurioft.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ghoocfxex.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gcoenrbmm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gdoekvbdw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grmoirwqv.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gakdigqml.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/godjhwdbc.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gxlxdshzi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gdawygplg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gqdaijaqq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpihnaxtw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gpfwstqdw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gdvhoxnfm.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjyvglpfy.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gbivszobo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gdyazkvbu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gydxdyjtv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gkzrgxstf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/grxnfoxjw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gxpbrbrum.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gkdkgtnuu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gdxdwqsog.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gypowqyoo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gcrvgzkqo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghkasqend.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/ggoefezxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gtckkwdto.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gvrflexes.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/girsaplpc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gezfpnjhv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbwaboymr.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gwqmgycyv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gahyfaycs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gicafahtg.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/goungboqq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gyyhlyfzv.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gourojtor.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gvgfoyahs.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/glivziqda.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gizlxzpsy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gqxbflmyo.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gffcyshrz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gcbtjgfrg.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gglbizcrj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/ggbuvqewv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/glqofwnnw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gcngbfteo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvvrcrsfl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gpoqtxhaa.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gafsqkexq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gvruupxxq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gdiahkdyq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/garlfdqsq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmojqyuyi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/ghaeygdck.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gxzrpygng.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/grjqjujza.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gpwzkxqvv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gwukxcyxr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gchazzoxm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/glflrhotz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/geqbitwsx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gjmwbtwkl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gvfyfutyp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/giwyqdkos.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/ghdoxmxuk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/guvfrfoeb.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/ggffejhta.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gamoaymco.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtifpujiv.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gpjzqjkjz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gotsqlbqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gofpsmddf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gqzvvddtc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gzrimdvvl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gmxtimrfs.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gglvuepur.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gyiuaspsa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gdhrkjrse.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjbgdiveq.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/grmaeqdyp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/grrukanor.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gwcoxkbdq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gjjcbzdco.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjinemsmq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gzdjybxeq.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gonoksxcs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gijqfhzbt.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gzsykgqlf.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gcyqnkdqq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gnvkkkbgi.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/ggkzrnwka.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gmjdmcgaq.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmkycvkzu.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grwsltppx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/goxqjkiwm.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gfonpewyl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gasrgtxct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gfdwjbfre.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvowlnk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxqvqrgyl.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gxgrhtbqm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gxlvxjrqw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gzbwtaehl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gpvcwtoio.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gllhgnqys.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gplpuonzw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gneachvfc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/grzqvkzqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gdcgydsmr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gpdeqsupx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gszgzhvua.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gpxsviopm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gpgggokot.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gvrvvvhld.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gjmvvmnmw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdovxsykp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/geonbfsoh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gwkoudnll.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gtgoljzio.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gczvjojtj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/guajoidmi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gsluhvjpw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gyeubsnrk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gsplxkief.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gqowmlrnv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gpiqnwggi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxbdzhzfs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gwbyagdfc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/guecovldv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/guogoiqsz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gurlhsmun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gxrlliskh.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gctuostjb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gziawusib.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gzohojmis.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gvciejdhd.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glgejltrp.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gpqcipnjm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/giozfeckk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gqlpkwnyc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gohwetsqe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtsaiwopw.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gedhtygwu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gizengjep.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gpeyoyujr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gpbgqxosc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gvtrydmak.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gvunfnpqz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gdjfmkayp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gwymkqppy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gmimjqeda.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gquzvarhf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gquradouy.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/goynphbxt.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gfsigmiid.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gdnycbvbm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmugagmwd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbtsowugy.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gevwcumzc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gyghedhnm.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwjtyzwhb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gsfpbkkcd.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnpvheftl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gxyqjrhdi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwkflakab.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gjmypanfm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmokwieza.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfmwfbfjg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/genuxgnyy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/grepocqtn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gbwxdqmjj.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/guxgnhdgs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gltpnetww.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gykooncjz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gnqxfvmar.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjcuouazc.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gormvipsw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gnfoknglk.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gpdnftzay.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gciddhnmx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/glgptvrdq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/grzkxqmbc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gwjwemsdn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/geldndwdo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gfkimnwds.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxnbpcgc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/guiafwqnq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gmngfdnho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gccewfhwh.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gpqaepvqp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbmturtfl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gdrzgtzwe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gitjvfbsc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcvnxgglj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtynboqal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gzgxttklx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gackztdpi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxjtiqmfi.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ghtxwwhea.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gygquthjf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwqnlskuw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gzxfbcgbs.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gbkudqymu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gnuwifpbs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gownraldg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/ggdancraa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gvkwyepnn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gyfsgkffz.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gfmkgcgvn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gkfasnorp.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkzhwmzmf.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqwkspngk.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghkzsvcoo.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gylbzhqkn.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gmnxxkwmj.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gfeyxphea.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gqdirbaoc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gtjaqsyej.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gjiavjwxo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gabgvcedn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/geetzziez.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqrqvondt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/glaphfoqd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gnocudcfd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gvmclecik.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gcvtaftrs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnpbgevkl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gfbachokl.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvlaenbxf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gissoqopq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gnhyfvdds.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gglcmekfx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghbdmbrgq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gjmnluvah.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/ghceblebj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjnjwzfou.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gldzkcuno.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gelopbyyh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glxszsoxe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxijektah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gezcblyxs.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwusmrjvt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/grrurwgdk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gfisfaljc.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/guycplfzs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/givevvjkl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gnuajzkyy.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gyndvqpev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gllmywpdz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gguxkqprh.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gosdajtxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gtmkhvcxz.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gqtncocrb.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gwnrqxtbt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gxgcmudbg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gqroqbpmm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtoqqefwm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gigjazlcx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/goiqyzzlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gzfbqhlph.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfakuqltl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gxpfzntya.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gnwwmblkq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gbkjfgigo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gkfjgplmy.sHtML


<!-- 参考信息 -->