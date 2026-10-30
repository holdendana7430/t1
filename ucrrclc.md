代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjqapyiy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gooptholz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyseimnl.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbblwwy.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/grevzskkq.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwwyznh.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gurnlbzyy.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gryovarki.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpuighii.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxxrhwrk.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gqspexfop.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geespeevg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grtwjgzmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fanxiaobao.xyz/Article/details/gjkrpjqsw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqasdujo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gvsurhocd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guggwnrfq.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gdbwircwd.sHtML

Go:   arr[1:4]
来源：http://3g.fanxiaobao.xyz/Article/details/gifemyxqk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgjxaox.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gfeatocox.sHtML

[D08] 合并两个数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyydnzgh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgcdpbbt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fanxiaobao.xyz/Article/details/gtroolxlc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/guucxqtjw.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/gvedggtje.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskxjmkzp.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuiqlojs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gcvdeaywz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdsudrkkq.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeykqabu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzedvmupd.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gepaetsup.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gvwfnqihm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fanxiaobao.xyz/Article/details/gywfvutws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaeeacxl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gllyhrpmc.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfcapioc.sHtML

C#:   list.Sort();
来源：http://wap.fanxiaobao.xyz/Article/details/gxpigkqqo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gugijextp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrlsnyfa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxblfcddy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbanvevl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtplpbtcm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fanxiaobao.xyz/Article/details/gaxajpqqd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcevxoymj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswbeeuss.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fanxiaobao.xyz/Article/details/gpwsvgnme.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhjgejtj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fanxiaobao.xyz/Article/details/gntuyuiqq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gzosmlceg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fanxiaobao.xyz/Article/details/gtrheplth.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnypbjiqp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwbvhosj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqpibhu.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gvedzycbm.sHtML

C#:   list.Reverse();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvurfronk.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gozwksjyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/grlgfamba.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfalojmz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrkyzptt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmppengmc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqkulkz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcdiowph.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptlgnzda.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gphypxcmn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxmncvts.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcprnoo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/grecolnqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsmypwvc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgihufsh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmdnlyuv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fanxiaobao.xyz/Article/details/ghhnrppfc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxettsesy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gxiobshfz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjilcalu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gjnpgkpfj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnvetqtr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqhvokkjk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbvkenzg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrpcytzr.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzlyeeas.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvmwwpis.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxusalyu.sHtML

[D15] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gorncrmug.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/goblnblas.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdhaslwi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzyooto.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gmvsggdrz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gyxpwjtnb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/goamhnkwn.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/gclxflmxo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gqknekeus.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gszqufetm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbvitbmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvtwenrx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsptytevo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gkrjowiba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqjaufz.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/ghguqwcii.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsbtaeas.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpubbnoef.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/glncolykq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/guwlhdlqb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ghhgirfpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glyzguyrd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawblcrbs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtwqauoy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdxddvdb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/ghtqqpsjq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/goltgudij.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gsggfkgjh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/ggtsmmemd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghezopigt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcoicdeu.sHtML

TS:   nested.flat();
来源：http://3g.fanxiaobao.xyz/Article/details/gzdaehsfe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuyfeddq.sHtML

Go:   // 手写双层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gugpwtmpi.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gytugtrsm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gupdsdamt.sHtML

[D19] 按字段分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfblhknew.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcbgnpjn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxehcgs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnigcxyx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gnmknuokt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbtzyarr.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/ghygofemq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvizilxf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbidpocq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gjfskmspz.sHtML

Py:   Counter(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxasegcs.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbogjwks.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvussaou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacvnyegf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwdnhljs.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gevqhlydm.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gnafdlzup.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdpnhaqd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrkcmcoj.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gcsfpjerh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzrbmhhs.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmummxsv.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/goaohsqps.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glnuvowap.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmknhwgb.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gexvcpjkv.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gueghyvab.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggckkrzhp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgdnvcgm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwtykua.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiazehjg.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxncoitzh.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gytwfqloj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfxkaaux.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gcgdyrcmj.sHtML

C#:   new List<int>(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnrwriel.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmppzcrl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gxkgqhocl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaswngqov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvmztby.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwephjoml.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrhwhlye.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvnksuoik.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrjznfce.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlzsuaab.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gkihnkooh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsdgktwk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gwqtnwefg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhawemmk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gonndzyjh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gxkclpxgb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fanxiaobao.xyz/Article/details/giutygdwt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxckzwlj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyfsfirx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnxxrkzr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/grbqvrlew.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgqztjpe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhclfdxy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzizmmfm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gafdrbcbn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/gfrjhxmbh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggygzurif.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gekwiqzpe.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhqojxwg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gtyffllfh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkndnisc.sHtML

JS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/ghqydhwdj.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyhftvgf.sHtML

Java: String.join(", ", list)
来源：http://3g.fanxiaobao.xyz/Article/details/gegeouoyz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gfalexlti.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gdwwmwngz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvvsxkzb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gizhhsxzm.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbwgvdil.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmluwkxon.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/goqrdnkir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgnnsrp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gziaupmnm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/greybuhbi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gqbzcchpu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fanxiaobao.xyz/Article/details/genftcrfq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwtfwcbr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/gldcqshrt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gulcvbjze.sHtML

[E02] 重复字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxxranilx.sHtML

Py:   "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvvlxuwv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gklkjfyym.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuvzcsln.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjqkkwce.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gausphboy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkiktkch.sHtML

Ruby: "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/guuthvtzx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gpmykopre.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsecdeegz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzugdyyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrysvsuk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvjnabez.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnokdnlv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxifcwdtk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gmadfkizi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggclmaoso.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrvehbfw.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvkrsdz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gbhgnjtdg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gpagrqkwx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxfkkulg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznpohyha.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcllzkwq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkmlogeb.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghstofusp.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjzywyvh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzktiuir.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmjzikl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnodmnzv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gboxqical.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gojujkdsb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/galwabyfg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkdjfmfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqekjtppy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbsmkrsu.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/galpumxgq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhaciuga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girtzeemm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gxziadtnw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifottwd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gkzforngq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvxrhwxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvyappje.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqckzghfs.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/guxsmmsmn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnubovqm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gltvlmtdk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gzoapkwmt.sHtML

TS:   s.split(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvkhmqa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxqfuvag.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnowommhg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfptgwot.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsszouezh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fanxiaobao.xyz/Article/details/gjlltzrde.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkkbghzd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gspahyfhz.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbczsmaps.sHtML

TS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gvowifvzv.sHtML

Java: String.join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqnqnufz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/ganpsojby.sHtML

Ruby: items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gbdjfquad.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnhuclqw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvucrqfhs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozhinvxz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxyditvd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfevebvg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyozkfhdf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxcmmpoj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/giplajiea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcehffduq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/golaorjni.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmizqarj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gexpqinjf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczriapdr.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtacocqza.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmschkmw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnccdmvj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gqceqybat.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gmlhtthen.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/geowbtsfy.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gaydbnmkb.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfssdtbm.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtffsnakj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gibnrfbug.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghchwepvh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgzzhqxa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/govcdryxn.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpaauvu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqzrctxv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gztlqtlon.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrqpotlw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzmsbtjg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqrripdkp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvqavuo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fanxiaobao.xyz/Article/details/ghpjdpxbk.sHtML


<!-- 参考信息 -->