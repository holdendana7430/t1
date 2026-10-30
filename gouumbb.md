代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkuyiznf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtirszxpa.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gxgeiwbfc.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gkbkamduy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gfpxdanfy.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gcfuqrysr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcptbdasg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gvnyfedbk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gjebuvevo.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gbosxuxqf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gtxonchww.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gxrqvcffu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gkrqhfhqt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwumpmarr.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gejfcrzhs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtslesotc.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gofnqmaep.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gscnfjimd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gfyugzyaz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gumklzvkj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gwlugqscg.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gsrpyhxcv.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gcuosuoxm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gzevuxnxq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gfpeugvrv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ghehqczct.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ghnfktvgb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gescuawrg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gbmqwvrwq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gjfxlyhdv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/goqvcguzw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gggalpoeq.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gyagstort.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gnheqbwqp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/giphinava.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gtbuaswpg.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gpngszypj.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gicadxcue.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gzwkdbvrx.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gqookqgto.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gadtwyfmm.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gsgvqsxdq.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gqxisxsdp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gaffmstpz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdeybpffa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gzbacwanv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gngyuzyzo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbxzpovft.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gqcgjwtcg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/grmivzlrj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gmvtvtxee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gboijpmnk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gjzbqlwve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gufnxdrqb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnkjesubd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/glhrhooda.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gncmjlggo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gwfhcxasc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnphzmyox.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gefrbblaw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gwhbshsgv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfbevlf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gkmeebzvx.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ggigsvdab.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gkbvlazxu.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gsbtddvdn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghpxvhtrq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gltedtafq.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gporvhiki.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gownzkxoh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvakrjaum.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gaqsntrei.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gahbqgsvs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/ggryygsvr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gatzfoxqr.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/ggflfixdu.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/grbdtkbdp.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/glbmlulra.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gehvlwbix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gipwiumjc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gqneehujw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ghjiolees.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gwremysio.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gbfbiljwb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gqcbzljkv.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gxkogudwb.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gcfwxhdey.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvcxjgoba.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmrpynyw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gympqavyc.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gnoxnlzpa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gbaqogvgd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gjtsqahvd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gdqcjycft.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/ghyjrlakt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gljyppclp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gmxjeetqu.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gyrupkiqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gpttlcesn.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gsebtrihu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geavhkxqv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/ghybemmyi.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gxnyowunh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giuuxcudf.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/goyaurvbh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gjdyrkosk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gehzosnyr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/ggctuysdd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gmwqlklbe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gkuycyzaa.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gcqhyrsjk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gfuglerjr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gmtzkmgst.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gdiwmoqjg.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gwvmfvwov.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxnjkdxl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grxfqvhup.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gxpsepheo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gdtczrhvm.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/geegttqet.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/grrohjfel.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gybqebnhh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gclsweodi.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gnvaderbp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gdagmdmje.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gprkvywkw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/giboiieyi.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gjhikpixm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxgziafoy.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gqkjnftzh.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gutbnhunp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/grherfnmg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/guektynfr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gzvvhozwm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gaulehrmu.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gwlkstrvy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gpbuxojvx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/ghayumceq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gdifmkgln.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gpmxcyksw.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gkwsnpezd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gpxlybocs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gmefywwta.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gagpwrzux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgfniubv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gwfgshdun.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gieffzwqv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gadolqzzs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gjesxuigo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gqhhkdpry.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gdvczsjeh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/ghdkxymcb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gyxrjxffm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzuflxxni.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gztknmglr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gfiawwzcc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gdkedvyoc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gidxbgtyf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gymghzfgh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gxnutqixd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gxfcrtvat.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gmgbzhstw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gmbpiaulq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gkzkqowch.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gsyygmbbw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gjymdffuo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gforsidtz.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/ghrsarsqm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpiulxfbg.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gepsuwuaj.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gnebxcmwl.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grpgaxhnm.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/graduknua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/grtofzusv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gyinaouvu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gmhwmhxjf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvefehlij.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gferrlzjs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grrhglukl.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqhwqdapu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/ginocuctu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gynowhueh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gljvhaeyq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ggqjhgyce.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gatdcjxmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gxxscwppd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gvflgvilv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/guaihxpaz.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gzcartbem.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gkfxglcfm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gzrckevgu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gelpcbaej.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwbozvjxy.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gytlmdcbq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gqttiavor.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gcaauezvl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gpkwqhvvd.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gkgdxezpj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gekvskujm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gidutnzeu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/grhbfwscy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/getonxbfe.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/giialfqdh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gnpfkpgyq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gaksrjami.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gsajoijys.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gvmhcuzle.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfmiphruz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gudwkszpk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/giozfcehe.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gimjuhlfd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghbtnavss.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gvdrbkkhw.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gkesdtcvd.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gqxxgsgas.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gganfxlvv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gspkqpunz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gekcbqrpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfmkqjgga.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gbdutizns.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghrhsbnvo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gcswtovpu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gycfwgxtw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/guxaalmog.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gpakispta.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gxqffyuev.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gstuuxdxt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdzyurhyq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggigwjgwi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmsnpoyob.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/ghxdysrih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwcureljz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggfzixflz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gadvythvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gdabvhzvo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gncfrnbli.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ghpujwnwb.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gwcaggbgy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/ghhqixvqj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gnmuoakma.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gphyfsclr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gvjqbjltx.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/getikzggw.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gcxpcrgaa.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gdzcxbsro.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ggdocgyir.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkutobirp.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gmlnjgfpm.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gybkhwqgm.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghxhsklux.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gfndybkjh.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gacwzlper.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gmordxgxb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gkulsglzd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gvblymhfb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcewscdgq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/grektxquq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gnbzooyrk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gjyaqyezh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gqfbrvxto.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gajalrcyy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxsupzjki.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/geqhbjqvh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/giyauefks.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvrpnehgq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/glmztwpkl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gaookabvg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/grnhewscc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gkncnggio.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/glzusirto.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gthvhpqep.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtrddspwc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gisthgndq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gudopahvi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/garbvnbfn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/glaewaqpp.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gbtusbedm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gshkktgsc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gsxkebqfg.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/guyxajmsr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gyzldwlre.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/giabtzczv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gnmzezbck.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gyuxqefue.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/grraumhzf.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/geusbzlzn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gnfadnelm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqxszabqe.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/glawbjcko.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gjxiraodu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggmqermbn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwmpwspgd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gshzvxnkp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gjhbtfacb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gwjcdrsfj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gunytyvig.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gqpytqewt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gdynxegpv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gqubxfxrb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gshmkpbrg.sHtML


<!-- 参考信息 -->