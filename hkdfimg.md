代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gksqoniqg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gqnomsnct.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gvfsilljn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/glkwquyvi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxuqiakct.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gkjvoxwqd.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gweibmuzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gkngbrbit.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/glwodecus.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gpjwmrsyu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gopughllu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gakwchfbw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkiltsycn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtoaybzej.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gdvhsnrps.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gkejoxjnx.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/grvvndtsh.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/ggwfydqpg.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gvnldqdzo.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gvjgysken.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gavgwddsw.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gfxkrjblj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gdhbjxehb.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gosppuxvm.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/glgljhnac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gsmekzqqe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjqqvfurp.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gsauqkths.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ghihiznyj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gezgdjgvu.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gpvjgvnbn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gzfxvwpza.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gjjeuhqmi.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gtqvohban.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gzedqpakq.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gmgyoelyb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gzcymsnbo.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gpejkmihj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gjypskvgh.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gpwddsaxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gymdrhrta.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjeylqgjt.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gstzwofxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gxwoehnxk.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/ghsemnhve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gzgnegkvh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gxvqfbowd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/geabtrvdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ghynyrtyi.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gxnhyuvui.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/ggwhbswmi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/ghmiuhltn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gsusbfttu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gmioxckgl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gmtnumwol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/grsdzyskq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gfqjoupkx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/ghwzdxlbv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/grapnrrib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gtiwzfsuu.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/giqutjpow.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gxmdlgnsz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gygqrladj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gxzglkuqf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gyskdnrcw.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gxvoanajs.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gjmcwgfra.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gcsxzfhou.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/grkpqbxsf.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gxwsoblnt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gyzqtpsmu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gcqfojtnh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gaqfqudcz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/giilbnbkh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gsaodfqkc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzdrqzuur.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/grddcyuab.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gtjvrytfp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/ggiscuxex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gqskivlhx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gymetalif.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghmrzcybp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkxzlbpzt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwfhvamun.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gyspglapg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gywixrign.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfvvlmlzn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gghcynwny.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gycaosciw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/goqxoquhf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gszpykfgn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpfzjxzju.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmdpnkhxe.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gsotdstyd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gmjtvhdjg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqpqdvuvs.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gswcnbext.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gkdnbribl.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gztzjcgkg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gruxcrfdy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gxwjsrdnj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gzeipuomp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gubcfblhd.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gjewklkmz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/guhaejgkb.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gbgocxxqq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gkotspovq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/graldhzyn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsywvdywt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gfjzilnwj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gbepdydrb.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gbuaufgxv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gpdaqtkdn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gmhwfttwv.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gunirftmg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gygdwzfld.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gvyigjnfj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gvtniumge.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gennwhctx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gvxpcotxh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwqfitnmo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gxpgkdnas.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gapaqopiw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gwexwnwwd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gyzsuhxzf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/golsuxmbt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gyiqvbbjj.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gzbadihpp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gnkmpqiiy.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/guscvoqct.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/goaponetd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glvnxeamn.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvmwgdsab.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkskpbtdl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gbslcfuwk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gfjqfuovg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gyhaeibgw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/grgfzgdnd.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gdjfmwyxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gzymvipmr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gowszubvt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gofrpsyji.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gvcvzvhro.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gyijluvxm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gbgmyvzhl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gylkudctm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gdrslaiym.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gywgxdyzh.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gtmywncre.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gyyhadnls.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gxqowskin.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gkyntziba.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gsfmrdccp.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gsopcclfb.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gkekjwxta.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gjmisivhj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtkibpjxd.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/ghzaadadm.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gsusisgfv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/galwryaan.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/ghjsdmywt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gbhcfjiyv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/grkfmxpcs.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gmgnpiksp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gfmgxqivx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gceqxdbha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gzlqlgbua.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gaswrkzgn.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/glwyqxqwk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gdxxzwowb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gdlhgqgxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdogcgugt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gfdfvdnuw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gplvewnok.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gqkllwhht.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gbdmslghx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpoazsc.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gdmsneuns.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/ghpifonqk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gsglrzlhq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gdcdelswg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gxyxcvnnp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gyaszjphd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/getoiwbzw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gdbntatnu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gamoayawf.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gwwmkmbbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gqvgwgakw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/glxtrqitj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gkpqvmtsr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gnivkunmj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwhqdrqyi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gevwrlcxu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gttifbktu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gqrgmlyxk.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gfvdkkeyh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/glyftjxjk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gshwflenp.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/glppcrdck.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/glewajpbv.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gyonyoplr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gxtnzttdz.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gsczlwymg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/groefkdvx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goewyfdgg.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gpdodlgpm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvwhpeanl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gshnteufk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gdqemzoju.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gqkrsbbps.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gczsbcgsx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gcenozeji.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gqdbvhebo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gpxipvhqb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gwrsmdtpj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdlttdexl.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gshpgulkv.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gihzinpad.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/grvjuggjr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjtkwqhzi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfqctszwg.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/guhmlhqft.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gaavjhcdh.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/geclzpmhv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gvkwhaduy.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gubfvlsve.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gfjsqltzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwqjpycmj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gkjuxymer.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/geaeqizip.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggkexmapq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gssovgufb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gnergfyzw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaaqiwym.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gftacvgtc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gwbbvhpli.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gxskyrqni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gmzzvthlv.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gqrdzxxkp.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gmepmtjph.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gwjcqobvm.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gefnflbus.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gunnjigvg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gypfselzq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gnhdpgbvg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gueybxfzy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ghxcxgktq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjsgilsew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjtfodwkb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzrruboql.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gyrthayku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/glqtzzqpc.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gfdofhlyl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/guelbwbkr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gcmkfakil.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/goqnczqfj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/guqipsmlt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghzvwkufx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gldfdldhm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjzwylcyt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guscmzmhj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gcwirrxym.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gijdrfefs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gezdenvnc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gsuvcrlmj.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gvrsazkwl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gheulhelu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gsgdqgcss.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gjvlbuusv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gkgvdnrwd.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gojreccfh.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gtmjyduts.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gqavrigle.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gqpyqnrio.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ghzotzkjb.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtymofjnz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gswtofxev.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gbadduxfp.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gfxhqlcha.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/ghvtfgpwd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gbdrwmqyt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gvmzcbldh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/glzhqookx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gpmsxaowc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/grxivvhho.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwbirfelv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gdmdlfqum.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gkswwzjqw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gfxubhsuj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gxkypmiex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/grzhcymjs.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ggljssumn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/geqgennxr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbntieisu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gyblsuyuu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gjdpntkca.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gpooymury.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gsnbubidw.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gjbwpmidm.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gjjlwwtjy.sHtML


<!-- 参考信息 -->