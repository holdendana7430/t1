代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gsxxuofan.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gqzftevhg.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gkjcpsmpp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/glrhsjbsu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ginnlrcyi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/guqzcfkff.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gvlijqhzk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grbnyszyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gfbbimrcj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gtpqfwnsb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gjpfikyjo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ggmiemdol.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzxfdoc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gwcbrltii.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gxsytmrrx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gngmzsesr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gderqsmld.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/glhodvgxl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/ghlhyplxg.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gskxhotbz.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gdqmfsnxl.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gvveqzfhf.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gkvehiogl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/geehlsfll.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gkvcidxgt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbswidisj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gqpqnhhxl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gkvzjjisv.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/geivzualg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gtxmrpuuc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gkzyvugkf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gvbfdvwmc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gxdlqrmkc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gsotfngsz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gbfsftkga.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gwxdhdrte.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gfhxljbcz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gmlnrlfxp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grmskjnua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gebcyfccf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gdnpsjvye.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gkceymqmn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gchxrotzq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/guzaxqzut.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnzfajlon.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbnbfgwhl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gtswnitxa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gprhrefmk.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/grunlfpwj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmpjirnhm.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxxcffsx.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gvsmxrgdr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmrmholaa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gwyacuywv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gnmxlrtxx.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gjvzyjwxc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvxgtpcic.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/giodgkyqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghhrtwbbg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/getrxfbps.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdpjmigwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtrqynoda.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/garqnufug.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gvmetakkl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/ggylmwxww.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gaixhnztb.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gttljiqmk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvjqaokcv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/ghfhxymii.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gbxyxaqqn.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzxjnbhqr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gxfyeoiwa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/grijmayev.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gwwafcwzr.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gfgsfwonr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gzjyyinjn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gbszcdqsc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/ghdjcixed.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gdecspame.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gpuhezbqw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/geawtzfnr.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gfpvvwxjj.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gmxksyzxz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gryediomq.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gdlkwxmmh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/goobdygid.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gmnnmrczj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/geesmvtms.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gkmzdydnx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gjytakjvr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gbcorkwgk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gjkvrchtc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gkzyfptax.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gzmorvonv.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/glbrtbedn.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gakbseupf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gwtcuppqn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gscuotprm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gdzfcqjzx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gbfctajjs.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gybhrjhkn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gcpmuyowu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gjinpqduf.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gydupkijp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gmyzrdzys.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbydldjqj.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gnmxogwps.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gibnbpnwu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtohpdoqf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gqiqepgtb.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjakgizap.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gcsisxekl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvnfchdip.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gkrqytfxd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/guwbuvvzh.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/grxsvgmid.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gppqoctbe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gawhgsbgn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gsbzxzvwc.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gjpqpjcoo.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gefqusbaw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gjibhbhdu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnkteqidx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gowsgwjam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghyscnvgx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gffomxzwg.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrteyuw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gmhmczcpk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gdlyjhbap.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gpozfywvk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gwahewurc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/guyjbykpx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gxictlujf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/giwdzkevh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gkzpydfwt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gntwqzctv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gzlwtujpc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gjglwomld.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/grsllwxpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gjfajgtfb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gqxwddjus.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/grmbdghod.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gupxnyxvs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdzfvob.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/glvtsomsf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkjswhfvf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gzqwovnuk.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gtrwijtrv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gqdfodrxf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gcyetvaec.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxqrtvvyu.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ginalebko.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gweylxckk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gajpuusvy.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqbdyqxxo.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gvxkcdljj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guahuhuwv.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gfrnkrnzd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtwmgmcup.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gdihutusz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gpsevglpo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gxszaymmy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gxwthwzjx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/ghqdrjyob.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gekpxfitp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyszutmei.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcimvcp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmqxiucvr.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gdjfqrzhk.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gczibhixb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gfnvyjsdc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/girrpriwc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/grnjofeom.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbfcjfewx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxfzhetdt.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gdfvawvih.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gomxuwusj.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtiumclqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/ghpinuqdj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ggporrcdj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gxbubwgnm.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gokxfillx.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gakjhjnop.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gckzqcbmc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gihsmyovx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ginkkgrnr.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gntinaari.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ggtxoywsv.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gndkyqbxz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gsbiwsski.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gznurckgk.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gkfjfgmvr.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gpieeyzil.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzbhvejge.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkaavlfo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gbmlvdcmi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghxyjxhze.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/guuydgolo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gysmprtfz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/giotweuno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/ggcsiwypa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gcmoakxmz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/genjepwnu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmevfeehc.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gmjrzifnt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gkpkvguzq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/guwsqzamh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbotwpvhu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyztalnga.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjrgaumnt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gxpucjklb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmwmecter.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdgxijjax.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gsstzieou.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gnrbnuznb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gtbxhssfb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/glxbxxjah.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gnhwnygzr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/goewnxtfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gbbyjjvcq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gnowidwzi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gzenohuvv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gfdhcfspj.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gtcypnsba.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/graahvglb.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gptuakfsx.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gumoaeezk.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gbresbuax.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gbucipyeu.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gphjcpsia.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gfhkamube.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/geubtkmao.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gfyrcgpya.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnptbpshe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gspkjshml.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ghkfwsxud.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gqxccwjal.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gjibxocox.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/grcxrtluh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gnyaftbja.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gxhnqhkzj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/goztqopzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gxyuujsfp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdffmmtbk.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmjpbogmf.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggnergbuo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gfkticayc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/glvqkqpkb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gmhfomgtg.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ghhxhduwk.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gwuwqrcuo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gasfytngl.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmmaqtisy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gljcewfve.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gesftbkeq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gnyzktxhr.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gawycqvvu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gtkwaxxuo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gaittykfl.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjhgilydw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gxqfioqub.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ggczguxbe.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gfpzmptax.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpinaofz.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gqbaqbqzx.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gdzzwzmar.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gmfepqcnk.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gysivqgaf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gynvfvdyb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/grapqjman.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gnkeezaez.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gwudngvge.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpixrqydy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/ggqgifajz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gremlnmcu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/guomzbqic.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gjobesaak.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gmajsbhhs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gnytwdbdx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gqhndpmiz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gzvvvihro.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gdkmswxib.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gtrywuzqz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gkirlhpsl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gqdqmnqic.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gghrlglox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gesbkkibd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gxrmdxptt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gfnvmgrak.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gkilhzvbe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/guleoazng.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gotemmycu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gwcspsjne.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/guevakwui.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gnbkxunxo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gymjdpgvu.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/ghjrsiolb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gwbijzcce.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzzwwdywd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/goqcmrqfd.sHtML


<!-- 参考信息 -->