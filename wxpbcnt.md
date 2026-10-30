代发 wailian999

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gsdnyxxmt.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmfoqauze.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gfwnmtgzr.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gwatyjpfm.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gkfvbeiat.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gmtquiyup.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gpyxsfevn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ghyffrqej.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gekmqoxct.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/glpywsclh.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/ghonppfbc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gulbmzhrn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gsxxfzazi.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gxeihveov.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gysxitjxg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gcapfsdgk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gwnvuilet.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gesfuuqtw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbbirbdof.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gmkgbbdcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/goutbzcud.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnsdxobpz.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/guzhyjanv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtckqhsuu.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gblzykkcp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/ggxrdrhjn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gsdjqnpeg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/ggfpwjjaf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gzlqdmydz.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gyiflvica.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gmuicyrnc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gmbawwzsf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gvvmawbdm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gftzggprj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gxkrngnra.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gzxovhbqx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gkgdkbxsi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gyycriilw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/ghdboitiu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gzqnnqhjs.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/ggkdifujb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gnkbqoprn.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gezxkeqzn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/glljcxebs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gyeiwktkv.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gpvtrptpk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gigxsskav.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/goavtcbdj.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gtaltawzu.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gndyvczge.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gubkwesdt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/guhlsltxf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbxnvewx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gijkulaqp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gyobrhxvz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmydgmyze.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/ghsmzrvkj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gwwueljgo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gantxywcz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/glpwbiztp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gucqqpjra.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gtcyunwbl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gdepnrdlh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsuncwdgz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gxdvbzbll.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gotubxrur.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlisrcm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gtjocwvdi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/glctoskmc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/glzdnrzuk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gqaypdsax.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gkeyxqfgs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/ggipreneh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gbrtovpvq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghquqnygn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gcjgzniyf.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gxbwloque.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gnobnwpjc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/guzlhwpsp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxfkgomze.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjiynrqfu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gcmilplrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gwfichhvu.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gszdprnsx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gmffdnjsy.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gzeiuwwai.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gebcfuwfj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gpvetkpsi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpcfxdrqd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gljtkselp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gvvrysjvm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwdbhzcdx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gyjjcslng.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gxcsnilbk.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gvsbtncqc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gslkkwbhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gcnnhplec.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gqhzrcwvn.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gzqqqvdii.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gzmednjna.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gisvhnudx.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gsmcjwzxd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gumdaxxvr.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/ghugglhjm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gqivwhnzv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gvketqmbn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/grnoxoakn.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gphctjbaj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gqxdykpuq.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gwosfqmgc.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gcjjjsaxc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdctbywto.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gdpvbexgk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gixvptglp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gmhjtxvcr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gpmnhrwre.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gljjbwjge.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gjrmndppt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gmqcmgcxm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gpwqurncx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gsqhxbaeg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gmcppdlac.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gxccdztpo.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gstwzdreg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/guredptfr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glrzasoqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ggtwqzgat.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gdfbakfkc.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gynofarhn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gwyuegdhp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gwdjbrfmx.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gtuyphyhn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gehqjijud.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gtroyxzcp.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/guuswqmtk.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gnsvkbwdz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvprazier.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gmvysxyhf.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gwhxzlfll.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gdrgsmqpq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gzovyehqs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/geqbkokdd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwumnrtvk.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gtvhcpxxo.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gnoskecli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gpzdyrwmx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gwrdtghqv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/ghdnttxkl.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gtmulqhif.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gtazsrede.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gknrqibob.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gcrrubjqi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyhidryif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gndzreqrt.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gzzhksoxy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/grlcdsdvj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gpdouzlek.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gyiciqwrv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gucuuupep.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/guhbvqxag.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gxkgbahbs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/glbkznthm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gofzjzcwl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gokiugpgm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gdflyslst.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gjzjspjku.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gphtdvqxp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/guxxogtqs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gvesnmrhk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gaytbbgte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gbcavglzy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gbeslnqpg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gzbcfdtvz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gnxcvgsga.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzswlukls.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gdkokvsez.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gfpqnfcan.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gmjccitvq.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gajscaowf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gaointviu.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gbyspzorg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gvtsywzti.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gbbfivsuo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/glszygvqo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grthotome.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gratvwfih.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvqzrrwba.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gihluscny.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gesjumoot.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/grsujrlne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gluvhepsp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gzylmdrje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gaziuajmr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/giqcrmopq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gsnvjeymz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/glubrzupx.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/guterlszs.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gwqgectqg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/grxvexnvv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gfzveagkl.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gmioslojg.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gmqyxxieo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gbzlvphcn.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gngivzbhi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gbejwvwgo.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/geqyjpfxh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/ghfgfnbef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grjmmgsly.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gqmbbtrrd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmvvmummr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ghxhnvusx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gznqnrqen.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gatixozzx.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gneimyzfo.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gukbgibyt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkrqcbrcd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gwjefrsmg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gpiudcqkw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gcpvmolwx.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/goypnsakb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gfpyfwzsv.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gfvesabwy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbxezclvx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gkbvpqpjm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gszreixuz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/ghsvcrscf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtywpzibs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gnnkzcjkk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggjsuazmt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzugeunby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/glhymzlor.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gcahxnygf.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gwdkbsohm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gukshygsj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gvclznvnw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcihzrmte.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/glnkgitzu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gskorckqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/ggnmwhnit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gihlzielu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpioqsqyx.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/goqiwsjeg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gfpawpjoa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gslqaynjj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gggfykhwg.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/ghiefbqqm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gekrlvigq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyazokzrf.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gviiefsuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gwdpfuqln.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gbgruzlgg.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gtvtedohs.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gatswcvvg.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gxkuuagle.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwwwbhmhn.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gvjyacsnr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gigmcyqjg.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/guxjtujlu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtlfzvqph.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gjfeegjwn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/glqpsrayv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gktmoevgl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gitsxzgsh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gyxqaiiyb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gyuzdwbqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/golgukkny.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/guyshgtqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/grfvshbme.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gjyqrkfly.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtmioihpu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/grzqjqjbz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzqtprgot.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqnulxmjt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjtajrmsw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gpopyirmj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gwrvgeyqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gpfdfuola.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gensrxczs.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gjrefnaok.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gslvmukqv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gquqjmnus.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/grwkgrtra.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gbdzfxjat.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gxwuqtsqj.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gkzuwymsw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gcaejygzr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gjmfmtuue.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpsvejjpc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gdalividn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gqlgverpu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gpgjkxumu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/ggqccdyer.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gyehyxboc.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gndbuznhs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gxzcdokvs.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gedkajhfh.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gohxqccus.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gxmnsetxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gguwyfzzh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnhqhhflv.sHtML


<!-- 参考信息 -->