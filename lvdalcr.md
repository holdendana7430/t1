代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gimvdwupy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/giutmhfeo.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gtfcthhve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gowawjtuh.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gmxqbuctp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gbcwqvvzl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gfinkqydd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gqoveuyhc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/grrbsugfd.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/goavjraob.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gajvutfee.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gbmowbkmf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/geeffkirt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gmktfckvt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gbyadpxre.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gagqczxbd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gnskzuzoc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gwrlojrdp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gqrvggxmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gpchvckmm.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gybncsdys.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdlccoymd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/ghobovebp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gabajfthv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gqtbcoavc.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gycjelcpk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gfctqqffa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gwoecmopm.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gvshuwyts.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gclckyxao.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gkfwirzly.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gppntafyc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gchrnlsov.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gpeurosad.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gonxuoxtb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwpdqimtb.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gqccogwjt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gxtpbajsm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gajntsqib.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/garrylwvf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gysxuujmb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/ggyicsgvh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gfpvygcra.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gmndwshms.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gsyqerobx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gzoeocier.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gdmzpcwin.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gfbkuitzr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/grvoskjrt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gkwhtvtjl.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gsrbsaixm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gwsqybxxl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/glfzhabeb.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gbwzupyev.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gesrfvwgk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwgsthenq.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gtygatjmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gbsutnrdx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmgisvaqj.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gebfunidr.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/ggmupwlaa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gwmgvonhl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gdgqlzzok.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gcyzkqngp.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gahzhpunh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/grgcynbrw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbwakohub.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gtjhwdndr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gybopqspb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzvtjxlgw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gawfhajsr.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ghwmmcvju.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gbtlhjlyq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gdeuahrhp.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gopwobfnp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gpslbrtkb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gjkanpiyy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gcbqrlzcv.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gddtxcedd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/glblwixbh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/grvkjfkjz.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gtlgbmsnk.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gzummzuqw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gumbyekko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gxksbmtqy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gclkbxgnn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/glwrbutkj.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gvhplwmxg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpubqfydj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gzxtlzecc.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gkbprbdbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gaqevwknp.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gutxcxrli.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvrjveznx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gcqalgqmu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gphifnwov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbibbgrgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/guwwyavji.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/guxtlkobc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gxmgzttss.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmxopblvr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gldnnvnxs.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gkyfoharb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdpfbgkbl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gmgidfbmz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gzihycmrs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gamshljks.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gclstsdmh.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gurngkulv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/ghomxmuvo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gjlfklczv.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gjzpqsozu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/ginimkivx.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gwhivfjgy.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gjoosivfg.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gcxapymft.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjrgeecnb.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsystfl.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvysygxjs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gmiqwvnus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gllqyoirm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gqklyrbqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcxivgysx.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/goyjlvdtc.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gthbifyie.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/goblcwypq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gpsdbdodc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gzlkwejau.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdjbgebec.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gplaadcwh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfipprlgl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/guiuduokx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gziekjejq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gcbykuhgl.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjsypabnb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/ggjzktrin.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gtdzyawkn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gxpvgwvta.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gfwpcwyqv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gnmmuqnky.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/grxfzrtsk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmgoqgsws.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gxuizlluy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gbaskhjil.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gyxfebyxt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gwtxkcpzc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/ggxqpicyu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/giititade.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/geaqmmsyf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gssgbhfmc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/grpgfavup.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/glyliikxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gltzgbjdi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gmqamexbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/ghvyhxtdu.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/goaxnsiwq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gawsrzpvy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gohatdcqy.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gercmvdfx.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/glpqmockh.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmbzczjjg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gkhwfivjn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gitrtedyd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ggzhandnh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtcxmmawn.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gncazsqmo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbdzmsclr.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghipzcxkn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gyknhashl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/ginbmuuwr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gnaljtmlp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gfytmruzk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gnmvvuqtr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gzbbldoug.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/ghzfarjws.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwagxmdqu.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/guwbeflfu.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gftbydpvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gujdwocmc.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gymewumil.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/glgkpjytq.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvxpljubo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/guecsiygr.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvituicnv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gihpprbnp.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/goantxiel.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/glerwnage.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gsavjohgj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ghxlfhgjx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/godvkpvgk.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwsrpsise.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/glrawsxhx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gmofgblbm.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/globomqax.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gjygbbgbk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/giryrifiy.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gmmiusxul.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gaxeinvdn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gbzbikuol.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/godcxzdtz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gkysatina.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gosiiujln.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvpoqqmkh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gakghkjma.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/glyxqeegi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/glcuavjja.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkhaejlka.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkwbgknyp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpzjzpofc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcjbmkqpl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gfwbroqvl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gypetcgxf.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/guxhcclvw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqqnabzyh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gchwxdraj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwwwapbem.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbnnewjkr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkhkbyzcu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfuiqzriy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjqyydfnf.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpiuyaoev.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gewppnqto.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gugfkcexq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gkumfdmus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/glfllvgcf.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gjrfjzsin.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gsjuaxkoh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gelqhemhf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/geakfihrj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gnivcyfhj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gjbcqhppe.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gygsdpuaz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gbfrsjajl.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gcgjkkzjo.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gdqolbwvh.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gqkgpkhin.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/glsuasefv.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gmquyizrq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjehqss.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gjuwjdpvh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/grucsxdlq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/geculjytj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gtjnkpqrm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/grhiuwhqc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gputgwtnp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gcoviimhn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gqngiajed.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gedxjfany.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gzxnaojcw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gsestggqu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/grvaxrlpi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ghviqtnkl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gebhblclx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gegipaoia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gvfcrepwb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gipswwlwc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gtfwjcqjz.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gksamvaie.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gajmneyuf.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gtgbtnubv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmcgibqto.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gccjysyhv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gmrnyscgi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gvecgpdok.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gwkrrvydb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gckkshpzd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gmklrrrim.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gajnigder.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gtaeemwlz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gkqrkgxfj.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gdbiekquf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gtjqoilbi.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gdezbdxkr.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gowzptnju.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gfeznousg.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/glzlnpmgg.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gkjejrmgg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gfpqqbgdy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqmjzbttk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gvxkxwcox.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdmuhnsos.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gzucwfwrb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhkctpmo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gidjgtpsw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gdngppjvs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gpaygnjtw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gvafkajqi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/glzqwjzje.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gskjfrqok.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gghrjabbn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/garecmrsr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gvzolhkhp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gzbcgoesm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/glknscljg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/ggzxsqopl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/ghuwwawha.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gvmwydwef.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gxianelas.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gcpnxryde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/grsqwlyqo.sHtML


<!-- 参考信息 -->