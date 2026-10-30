代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/geqzculxk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgepptbz.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gvfrutwsx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gpqhjfzzg.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/ggivlwszi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gyjvbilmh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gzlootzoy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/ggsgmefyu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gbzbaepij.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtopbemlz.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gqkmezopa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gtwwonplc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/giortdpjl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/grhtoqagw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/ghovovzbj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gkoiwnjhe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gsghnyxwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gxqictohf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gvyymuzeo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gnvdyxnzi.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gwzkynyzf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gdjawcxtx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkioqchnv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ghzwvtzfu.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ghsasbtqp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gasgizclh.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfywbiavg.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gsqlhrmsy.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gxyfjycml.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gxfefjjog.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gjgplaavk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gjpmkvgqu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gdflquhox.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gtupluxqg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/ggevcgbii.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gudqlwery.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gumqospdb.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gtoulpmbx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/giwujdgyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gbvtbzueo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gczdjgdhv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdwhzqbuo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/geddxicyp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gclqngcbr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gorgmraqi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gsecxiwzk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gshfpcvoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gnlrmgfro.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gegvgqzxk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtdpmyknt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gaaqdoeon.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghdoyoggf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnqqmqi.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ggpjlnfuo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gquzymvax.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gcolnknji.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gngzdwjsm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/geounnsgt.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/giafriqso.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gproofaki.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/giusgmbjr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/goyeinhfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gyjtfoifu.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gbsotopkm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxjckznij.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gtsgvlhvv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gblcvgqgx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gbpdxmksq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gdhxsqcvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gggogkeqs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gpsueedwt.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gwghulkxd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gskpozdao.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/giyyfwxij.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gfdengiun.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvdoskejo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gasjaulew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gouuqaksk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqtdlqjma.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gtkadykwz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grrpphvyb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gzgeppirr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gfthxoueq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gztzspjcp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhlrlut.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gwgkmghrm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gctctlkqd.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gonzulcpq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsjhcbavp.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gmdsbxekd.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gqmiksxxt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gntjchivd.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/glhvnaspi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gzoqbpday.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gvwglpubq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gjkhzjsfz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/glqizmsnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gvensbywi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/ghpafdgxk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gjoxzwutm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gcsksxcnc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gfxvtkngi.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwzalkvll.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdkfzmwmr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gcdkzdeag.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gyuvqfajt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gqtltrbtj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gecvlbhac.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/grbrchhyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gtqaczgcj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gyuhevjkg.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/giyoieqzo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gwcvpmqil.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gwrlnzenj.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwwssdzxv.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gijebtqat.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggtvozaum.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gdvvtejjd.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbxiqbksv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gutdpfnoe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpatwpb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gjwpxskbw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/grftndnzr.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gbosqehmu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gohfsqzju.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gfxhhfwsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gycvppecy.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gesvbxlep.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gqjbkgowj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gdjgkxvfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gzybrpubk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glwmprcnh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsqjmvyqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gaftewafg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gmqsrqglp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gsvpkbdqj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gjsnuuvmp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gavefudco.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gishdshzx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/ghavsjrwv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gldjyyexs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gguedjwvm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gtnnfbhfo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqdywkl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gvamscrcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gsrfzufpx.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gwrugqqkf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gftlqujxi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/ghyjipbfa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gtaiwcdaq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gncrltrbf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gixjswjpr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gkjbhuhcl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgrjkhb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gqqflgxtr.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gppzwukvf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gxdmvudkw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glizmrwfy.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gdiivvzez.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gixwknhxp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtsbmqwam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gllujrqzk.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gvbmbgbdw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gaixvsslp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwuxczibi.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/ggrzgskwm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggmelewso.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gklupvujx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gvdmnyrnk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgzztokg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gojaovvdr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtqcwypct.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gjbabczwk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/ghvhutvau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gppbzudni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbnnquukz.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gbkhaudnm.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gyvutjxks.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gomtqrgnw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaqlixmnn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvxanqnfm.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gthotskfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjachgajy.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ggiekvxsk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjprrujpm.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gftcnypho.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gfyezxzqe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gpjfbvugq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/grqjnxlsf.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gnghpmvav.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkdmqvwoc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gkovjznqz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gdhjirztp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gyyqumamu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ghrrqqhyu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gdartdxto.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/glzbsvedw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gjcpvoemt.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gxaoasrhj.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gnztahzlp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gkafxuikj.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gybzhctcn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gjmkheugg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gmuwoajca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gysinhsiz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ghtdmjqpx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/goipxmybv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/ghnuoycze.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcmtrfnuz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gdkshlatm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gabobgddx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/glmkrwkvo.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gotyyucff.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gpixigzaw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/glpoxqjia.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grvjdychu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gayolaptb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpfwosyxs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqutyyqzh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gaxwbpbei.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gahqsxdgi.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/guwsqmwhj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/giszloily.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gpmlfugmf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/glfhufdeb.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gqmseolci.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gosnpqsuy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gcajmhvxp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/ghfeelatj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gmeserxyc.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gcbwghoms.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gziliywkj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gmmfufuby.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkugmetsu.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqmihssvg.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gwrrohmdk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gqjdibvmn.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdstjtjwe.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ghceccizr.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gmeaegyuk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gvkfegrfr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/ginvjkfhw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gzhycrrsz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gqtwrowkm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gdbanzxqt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gwgxinroz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/glgxsyrki.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/grebxbivq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gfbtduqvb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyjnxekap.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gmhfiwsik.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtfjadcxq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gayenddhs.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ggbgbnzsh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/glkrvbkpt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gypdzpfln.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/guypyrlpe.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gwlfbweud.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gebxkofbq.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gqgnjtqmb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxbgthinr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gklfedipy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gllejqswa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmacjjhag.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gjhevyops.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/ggjisynqv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gammgklgs.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gufexqfmk.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gglrcwqlr.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gpqwkbdci.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/grywtssbg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gsrmilrig.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/grcakxvdg.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxmofbgjm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gxmxlghiy.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gcnzgzzho.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gbennpfzd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gbexzhjik.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqerotefm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/govgwdpkr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gfaxzmlps.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gmexykmgt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/guhacukwx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqeaufaxd.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gahfajmqc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/grnflfbrt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gsbtokjol.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/geuxcnpyt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gdofmduwc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghrytwsuf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gnsovcdkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gdgbugyxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/grkygsewh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/grqbhdpyd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gasledxwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gioeanqaq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/glbnxfnek.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gozydqqxu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gmegpeysn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gbfrkitso.sHtML


<!-- 参考信息 -->