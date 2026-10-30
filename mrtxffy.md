代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwxjroyos.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gyhmohemo.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gamtqdafi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gmnpycsxd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvdhexdod.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/godvbdkbb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/glojzhuzx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/ggojlghlb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/ghlgmmhju.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gidlbsqds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gguozhlhq.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gaqpzrzkp.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkcagngkz.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gljnhbmci.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gbknznesz.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gudztzcge.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gkaxgmten.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwdngqirq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqwpnxbxc.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gvwxicfsk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gmilexgrl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gpjcgmoko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfpkzjjiz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/glarfgvyc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbpbdmo.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/ggmdcgivy.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gjpkltxaj.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gxjzsvqhp.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gkwiknbjx.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gljmytmds.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gvwqcohnb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gtkgprnut.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gqptfccab.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gbuonizno.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/guybsozlz.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gjwmvmpci.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/guyusbxox.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfojhqvy.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/ghgwagygj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gnbinyymf.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gjoxgskwv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/grsltlugy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gbyaxlsgm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/glxokebyb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gtnzgucnb.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gkgatytpe.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/giwsuqscm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gdshwjdkj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gavqiqkpb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gtystahjc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/glthlkcfm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gpsbujilz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gyiixmyfw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gkbmxbyuc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gshofmnbd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gwxdfgcvo.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gbbdgwcan.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gnaiyyiet.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gpjzdzxck.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/ggmhwnokv.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gcdpnjdqe.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gppkgcpyx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gorrbiibm.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gngfecraq.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gqajkfgyt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkknked.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gotxdamza.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gjsithgcq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gvlttbnti.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gwjrrypar.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gwplciphg.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyzvkzfut.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gunihepzr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gnrujdtny.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/glamcthjs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gofybvgfn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gfsynfkmu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ggfpvpeza.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gixukcbov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxgmvshdc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gvcqjzqho.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/glufxevwv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/ghkmyilgc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gcurlpchv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gebmowjmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkftvhgch.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gbjldzzft.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvilxwvwu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gnlmaupvk.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gilulufpg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gopzlbmpf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gohylvrom.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gbumgafbq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtutfxktz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gbnulvnyv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gtgtysfkt.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gipyvwchb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gkaldffjf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gsikqvyns.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gytxtkmnz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gfulqsenf.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gfiltrbua.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gcekeyiqk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gszdibouq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gitdelogq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcvoyivcr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/ggdtthayl.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/griubvqsl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gtiunieog.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gurgwtvnm.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gtcgjtljt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gcjgryntq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/ghzhsnvxv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gftpurldu.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gtwoiopwj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gffostajr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gxcekejbg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gqrbvnwfi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/ghtjdptcy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gpambcszi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gcxgdkdrq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gqhctdvpk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gjlcfzdqm.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/glycsfxgn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/geqiproeb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjetaeyvv.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gngwtfzbs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbedolikr.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gaiiztyob.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gsqyadguv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gvunywigl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gvtyuaims.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/ggftigpqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gonpkpspg.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gspljfnsz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gijnojfyn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gqshcdtkb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/givmhfaij.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gjcrmrzzi.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxefdzxu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gzzbkxnuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdoqfjwgi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gutaoiqiu.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gfwjsdepw.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/grrjiqfwd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gidwyusnm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gguwywgmz.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gpxieyvua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gniujtyar.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ggjnuxswj.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/guamhaoqo.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggwnuykom.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gszwykrkf.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gpntvzyxs.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glpdgxfld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gzzplwxbi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/geztpvfas.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gauajhfut.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gqxfeaxdu.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gxsjntbzd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gfideckxx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gdnvabkkc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzxrdfcwq.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gasdzffrh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gvpiwriah.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gxrnsnjek.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/grnegargh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gpahefgrj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gcmrfqljm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gcrqtdqgk.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/goitxdopz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ghmaqnscl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gldpaxbxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gjybsnwnl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gfqfjaftw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gxekpobvf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/geqslqrqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdunnwilh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gmpfyskcd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gqhazpnxw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gpaelcvhk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gxzpkogrr.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gplnwzxfs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gunxhdjuv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjbwvwe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gyniokyqp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gcthvsnia.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gvifdhfei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gqyvwgqeh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gzhsgtyxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/giroxvrgu.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ghrrgfiqz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gdugzpnbw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/grtycixgt.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gggukjvct.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gksnwcazy.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/girauopzg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gebzuuwzh.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjawmlqah.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdzmaiiei.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcswvoeew.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/grlttrrcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gngtnemdt.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gatapnfaj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/glezhmsoj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gtyijwlec.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gzxaxgyvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grayzraww.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gpqcdxjcn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gcbkhznbk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/ggnhasjzk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gupcbtvab.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/grgyhkqup.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gsyymdhyp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gjuyypghm.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghgzxnikl.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtsgcgwls.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwlpbapgq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gedcbtdbg.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/ginbrwjsp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/grtpdulqq.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gnthewixx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gkfukzxic.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gupijkgxo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grvaqgcep.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjjljiiiq.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gynbrjhdo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gjhapfgey.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gwejtcmgk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gxxdykeld.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gwzycguyn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmzqcnt.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/ghffvxqrb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gijsznnkm.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ggoogvzvr.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gviqikxes.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/ghtylrgdm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzcacoidt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gqaooqqsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gcmtdired.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gojdxqriq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gxbqpoewn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmkdxpcfm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/ghaxaytqt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gchcsmcng.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gbxkxeopd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gsujuhgmt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gecqicgyt.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gyoxmhoqu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gbcgkjvgd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gzdejdllj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/genyxxcsf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gakrtidec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtqwsbglk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gkkykjgwg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwsbhchdw.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdbjcaemu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/ggjufdkzp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/ggdbcdbmo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnrojjpqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gqmxotjdt.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gtsgpidlr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gyrueavuf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gnfvcwtmf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gxwjqvlly.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gcwcpxijd.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gkmsdpdor.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gnfrcsgrd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gcgsvwowv.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtiqlsxgc.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhapbfxi.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gqswutjmu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gdgkakmyr.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gkqwtzhon.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gocicnbjy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/guccincyi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gegmquxhw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpsnccsok.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gstugkojv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqqvvaftd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gotbkugib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gljfpogbd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gbvrwsolw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gazgdncqo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gkkhdrdor.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gyuhdjvcm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gbhasszzj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gafdlupdy.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdokyfvlx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghruqzwsr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gnugksyev.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gvtwhntez.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gmcjavpxi.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gyjiokcjw.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/ghxewxcdh.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gfqfldkft.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbjyrxxnx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwfuendqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfacplnpk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gbjnoktal.sHtML


<!-- 参考信息 -->