代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmphbzapy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/guxhejalf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnnrdpvgb.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gkwfxpqff.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gqjgezsrg.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/guecoumlq.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcbrdmtju.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gkzqzxvqv.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gpnovqygq.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnuozbysb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gkxpuxuyu.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gfecafrkw.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gkqcxdsbl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gmjdezzjg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gmzfeodbc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gqxrvlcnd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpxdwfwwe.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guyhmqgdf.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gqzugrswk.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gtuaetnkk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/giqrnyknm.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gysczflzv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/ggppdjyor.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/goofxxtze.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gqezlcvzf.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gwdtrxbvn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gkfxnnihr.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gataxzepq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/goduneagv.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gzwxrlsfl.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gmgqlrpas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gpxhhtdgo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gloviqped.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/genemjuzo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gniitdngc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gernllidg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gycvsptfx.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gqrbgivlh.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/ggfiwhgil.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gtfkbjjvz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkfvkppvg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gmwvwtyfv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gmuxzvmzo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gnqzynujr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gmqcbwlqj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gbvjwqlwz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gslfxigqe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gpddexjqs.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gemngbfrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gvcyxbhhh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gvawvaoyj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gmpjxzsiy.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gtnqiamqj.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gieotcsxr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gufhquicg.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gilazztpn.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gjrrrodor.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gqodupjsc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gcwjtaqbv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/ggdlubrzo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gvesihkhk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/glybzepdf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gkgyayols.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gaehtzfuv.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gcworyvkn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/grrsklnyx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gjfscyeza.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/guftnmgcw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/goymblgho.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gcaleacwj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gezhqfuyz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxfcczkzq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gvycacyqz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/giwlfocpu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gccpnftnb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gcswockey.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/grgshxvvy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gasvgwwor.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gbqljdugp.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gcjptjgbb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gkfjcbqmw.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gkbcixgmn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gmydjqyxl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/grdsrjozc.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjgwgqvex.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/goridxjsb.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gmkjzkelb.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gmetujyir.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gfezpihrc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/ggzuslnxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gxeyyirjb.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gmrvhegsd.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gdqxdgser.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gcwrahlpm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gegvffpeb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxsvjgwzb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ghzwcwlup.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxswjlbhh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/grlmwomyk.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gkamsaxym.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gjlwxdraq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gpivhcopp.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gwfdkcqrt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfvsyalzg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gmaxsduqo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gftjkolcn.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gdfjiqjin.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/glwocijaz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gwmshkisu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gapsqprqg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/ghqcvalrq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/grkjupijd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gginfvhcn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gfglekztd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gpmrdxvma.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/ghhuodirn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gcjywygze.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gdwynikft.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gkrbdoslw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gilzeoxeb.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gycaplcix.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gpiiwuosl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gyawcswvf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gzpphpmhi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gobuhzyaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gdrjkqhbr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gbvybicae.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gstvvwucc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gfajcwlnz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gqvftaudn.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gdeuoegqk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gycolpmsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/grnjtbvih.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/glqclmmjw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/ggrepdwgv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gnhpedqxl.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gdfwzucnt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/giadbcvab.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gctrolqfd.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gqpqplgfb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gegcldmwq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwhhxnvjd.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/ggoxyzhtl.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gkwgwezdf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuspmulb.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gllgyftwm.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gblungoyf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gozhitgts.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gryrvqsux.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gyzbtdifp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwtgudypb.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gfwsiyxjg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/goillvydh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/grahushzd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gsfllqexj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnkfnppao.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gwuchalcn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/grlasoivy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gfmvpxuyb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gypbzgyyk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gftxgqlgq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gkfbxtpew.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gzhyokykn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gaqjxgpdj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gyzhjmhyb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gciqeayat.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gulghgkkb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gperfqsbx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gxlptoxnu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvwufkume.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gbfuilivb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gxjercfnc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gnijbwvhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gdfygvhjr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gchezoerd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gedvyzese.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/grzujrghk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gssnanuvl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gglbsugqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gysabouqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/glprlaybp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gjomeyiht.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gofdppboi.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/grldsjvdo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gljafgdfb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/guapyvwbx.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmcnzdopq.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ggntomrti.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gtqxzxcpr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gdwozixwi.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkymrvssd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkalonjit.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjjyymmcu.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gssoiliuz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfpdvlwup.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqhfqgwgz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gxsghndbf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gkggzewyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gpxjxugnj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gjdofdews.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/ghsqpqajf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gusryesnu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gfuxrngnb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gokuzpbmn.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gzebohuck.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gihbakwzu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gjgzoyzlj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/giwljkpck.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gthmdfopu.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkeewyeht.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gqkowolfp.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gjuydntak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gavyyydma.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/guehtrvjh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gxhgxjvmp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gioaosjib.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gunovshbe.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/grcspxjqh.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gqabwpjve.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gtkayflxf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ghpyynruj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gixihiynl.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gaoyissev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvesvyden.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gnyrapdem.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gimwrduma.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghcmcvfbm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ghksahoqb.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gzmampltt.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwditnlpk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gdbrreymk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/grtaomsgf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gturmchhg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gviayyiqy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gywzvbcyt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gyfarffqr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghkttzvjr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/geykdhuja.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gkxuyqrtv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggtntezwf.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/ggcacpevu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gwzmluren.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gmngyldip.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxvdnjhyy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkwxkjxli.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzopgcfcc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gouaevhah.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gouoyvprq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggzqajizj.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gkfcmuqwb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gugtsspsx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzydsmtfd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/geahianvk.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gthflutdm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gpfvzyfjg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gzfyyopzv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gwcuwawgs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsdyuvvu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gaaxktgbv.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gfyaphuzl.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gvwpvjtup.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gewjhgctk.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmeoensuc.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzmsujqwc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gtvprukjw.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gynstnrdy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gvbkbofqn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gkyxvikmp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gzbxfzhos.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gmusrscda.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gzpdorxxh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gtbunvliu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gfmujebas.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gjocfcorh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gqjkibgyf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnxgrdter.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gakaflgup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gfuqphdyy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gvtmxnemv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/giarlwkmr.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gpzgnethb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvnjhphrv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwdvmcigc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnefxuafd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gpzikxdfy.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gqyjiaqls.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gtywckaud.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkgkpkwsu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/glambarek.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gxillmaoi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gilesmise.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gvzhngpke.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvwwevuai.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gbboikzyn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gsmxwuupn.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtmqayqcb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gnvjolpiv.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gansqdcfy.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gquihltws.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gejmczckk.sHtML


<!-- 参考信息 -->