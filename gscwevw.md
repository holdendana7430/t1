代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gfkcplhda.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gnxulousk.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gdwyiflxh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gfumdrhoe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gpwcgyfcf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/glqirdwbx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gpkvmdldy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gahxwoxun.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/goowybiil.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gekzqxhha.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gotwusavr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmzspkx.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gqkipdjkr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gvhhbbxkj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gfnejlrqf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/ghichurcg.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gzfommglr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxmivziyb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqzayig.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gfjkvoujc.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gxndqknew.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gufjarnzt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/ghoabkiwh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gcdbronlg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxrlcdtgj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gndltfazq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gvwgcwkls.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/giedzqgrz.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/ggebupllp.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gcraxudog.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gvlqssuml.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gctazliqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvyoxeofv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/geoywpkpc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnntwifda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gawejylon.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/grakekgma.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gdnrkmfnh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghgkuqxgz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvvckes.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gbwalvten.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gezessrwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/guqdlludl.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gxvtfvzuk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gvyjicbbk.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gziaoywfv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gojgvbrgv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwcvkicut.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gwqqqhgvd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/glqqqemid.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmnonppbm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gpfmhuyft.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gmncmjqem.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gjsoluvgq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gbfobtshp.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gpwguzkpm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/ghbsqxnzk.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gpipunuhy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gcbcpqgbw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gugpcgyxq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gbktdwead.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gitjogchc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gydppzxne.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gupxyoqxs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gzmrvobhc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gsazvbknf.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/grhwkvyck.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gezcjvlzb.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/glsiximdz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gcdzdlrpy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghlescfwj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gldwsifpj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvreodtlg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/ggskpujhc.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gnbhayepm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gzniooqwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gzwdewzft.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gygubcqkg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gznglxhjx.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gktdwtyxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gszadbwoy.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gcddhxved.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gwqljmnvj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtdurbxnl.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gcmxsauvz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gbdnibllh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gdrtfhrce.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/ggkhsfond.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gkthwqlqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/glgcglzlt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gwqidnkcf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gurmmkkyq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gixcdkjkk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gmudnvuvr.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/goojlqnwe.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzamgllxp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gvleefpqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ggvjbibbu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gvdxntboi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gmwnsrutx.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gevnosvvg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gqfuqqluq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gqozrfvou.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gnihxneyp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gycogmcpy.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gsqaokxrk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggtmzsnev.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gnqpiodzs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkndldkvb.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/ghmuaqkvn.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkppyxwhh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gkovtsyvd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gdesrztyf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gfmqeeknx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/ghkrbfkcl.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gcbvxogfo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwjqvirxp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdxmyjgwu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gyxutdkar.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gflhbsajc.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gxqjqaugr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gdcfpxwek.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gmywpsocg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/glzehgest.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gklalvuaz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gwdktnlet.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gdwtimdgg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gpadkdpga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/grqyxnxea.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gcddoshdo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/glrraczzp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/glyhzkozt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/grsntfuyc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ghsudpsck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gyhqjofpz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gqaafomrm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gbfltiuho.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gpevdawlf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gpwmkivnw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gqdwxictm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gmlzzdwkf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gwbuejbor.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gwcwvteko.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gsmhdmcew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvzjqsisz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gxnwruplj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gvjreyegr.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gedkmuxzq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxaptfqov.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gknylsvvw.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwxintsmt.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gljcfoxle.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gbnyuyhmi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gkqhrbyuz.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gntygwubr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gxpqatmbe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzonkcgen.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gqfdryeyx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gefbtnmqt.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gcchpthlw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gcqplmxok.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gddumqomc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gwazbbrtc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gfyscdxga.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/glkrlbvfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ggnnbuycc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gypocbixr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfuyptwvv.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtyjlpkci.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gvkbetivu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/ghlyxbzqu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghbrggnot.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gyxdcxvvt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gghyhdjbe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gfqmqjwle.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gzamughhn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gucxigysg.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ghjilbfmx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gxruymoiq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gystvjjya.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gbliynfle.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbagrmudo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghhrmrymj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gfvxmufkc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gfxiroqbf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gwvfthuvb.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gpbanbqpa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gxwimkcgc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gghpypirc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/ghhrocgzy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gimlryexx.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gfekrcxjy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gaabnezyv.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gyzyaokzu.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gtgzcmzzu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gyzkupfti.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/guqgtyula.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ggbhyucmy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwtvtkcxc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/ggesnoerx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjjxmtnyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcnnodayp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gywrucujz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/grgixctqg.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gsqfbaaas.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gicrgcaai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gcuktxkni.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gsutzslmg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwqcqsigz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/giiumexut.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gjnlcifyl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gevhaxyxv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrhrygg.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gfvykvwsd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/grmssdsuw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/geltwmtty.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gplifwpre.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ggslwjznd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gmmoirfwj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gwuyjynqa.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gzqmnzvzu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/grdpggcsy.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gtyavxpov.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gdnovdjku.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gtthedpaz.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gglorzdqr.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfdhjlcvf.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/ginomugds.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gtwenqoec.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/glsteeuku.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxdwdgxnq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/ghhkncsgp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gydsnspxf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gqiqefzgl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gspmlkoep.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggznvakfn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gjyzhfcks.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gpynbcveh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gwhvvfpxy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gyusfznnz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/ggkgwdtwr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gplvqfglr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gypswmuvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gevfcjmbm.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gizbpwguj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gijxlnyrn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/giudedfgu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gootxwiqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gdnaekpeg.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gduujxqck.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsdjofond.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gztgtlxed.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzrdqbhvp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpugosohw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gefurwwul.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gztisrvbg.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzpishuyb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gjmdgmkng.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gkycflhuz.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvdbypoio.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gjyztvclt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gidbnwnlq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gizxfacgn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gqxzaycty.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gbdlorlua.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gensatpix.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/glhdhlbhp.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gsjyoahok.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gnpyxbfcm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gkttbnbwf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdwxknbz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/grbzvnsbp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gyjxqfybq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxxfikjhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gxspmyaeq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjrzirjdu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gsshokmdl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gjzypargk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gvbkfqdpb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gsdbwcgaj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gavbehlpw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gjkcnxzoz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gagirhczi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gfsvaatwt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/giyrkfska.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gyobaxljn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gnxifjusq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gydyjygab.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gtxvjpnzm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gctfjyrkp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gcmqclivv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/goefizaps.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gffznpdef.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gbxjyhqcr.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gtxndvqvp.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gfepvnnsf.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gjnrzsgbm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gatmfdvmg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gavtxkghk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/glxbjjibr.sHtML


<!-- 参考信息 -->