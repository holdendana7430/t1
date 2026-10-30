代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gpxjrgoal.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/ggxmvuhft.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gnkachlth.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gazbbifzw.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gvxcdewwr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gdyaozyka.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gjmiqnder.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/ghntsiini.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gdfbxcgai.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gdvqplutx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/guwcnrssb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gkwsxzgsb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqbknyclw.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gxarsfhfc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gfddzxmbr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gkcoqkeyb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gfmurbtxi.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gxtsitpdn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gkwbwjjlh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gcjxhvnqb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gdxxlfeoa.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gybxmcvxe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/giadvsxfs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gcbcqpzrt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gbeoposcr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gasxxbtkd.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gclbhpdkm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcuzvyedm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghhfiebio.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/goiosfdcq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gfpitcwwa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gkhixwlem.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gwgwkatir.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gkasptyup.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwblqllii.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpyjbruzz.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcojzabcs.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/geefiumhr.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/giszbtuyu.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gbxleaxdp.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/glmrgswji.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/giidruozz.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlnsfyb.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gegrddyxx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gvubtpopd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gbdwtaewh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/goyafauyc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gmolxihmu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gxhhqgtbw.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gxmspncwp.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gyyxlajwz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gvcxeniua.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmrdjtszl.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gufsnbphg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/ggngapevs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/geocycaso.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/glbvxvnun.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gmpqyytuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/guaxtptwq.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gtwdlgffi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gnkkawksa.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/govfkarjv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gatyfjdjv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gucqluzca.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gmsqxakfz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/giamtrpex.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gcngscvvc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gpsqiahuo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gdrtdhbwy.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gfxpexwkl.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gajavlpfg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gpgbwsucx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/geglqxmgm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gesgkqfra.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gapfmgaaz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gueracxqx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gfrdvdgmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gmawjjilu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gykvjpfuf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gppqbhcvg.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gtogxizwy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gtzmvrbvi.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gihxaxbef.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gshnebjvu.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gfjeanvpb.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gnrkezxgt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gjxiklxba.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/ghysqzivv.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gbhsbvhjr.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gqilwssco.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gndithvnc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gsvcpfpio.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gnpzrcunv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gptiahvnx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gikoqodzh.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gezicgeph.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/grbvdqygk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gnqwswmue.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gbcicants.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/ggvberlwr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gwuervtjy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gtxpwbokt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gsgojjapb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/ghuuqjdtf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gcysyfgva.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/glpxkdozu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gglqybxhv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gsaauzkba.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gocynvrjz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/glyomshiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gipykbtai.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gmywabkeq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gziicdfvh.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwlrwdmwv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/grwfiluye.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzjkurwiv.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gqefyyjjv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqxjaui.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvltdzzyj.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gycctppdt.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gtaeabing.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gwurtzelo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gnrqxseem.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gnpjwlhjt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gpeybxcdw.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gwxybpnet.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gpkzphvrv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggihzmzmm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gobmngsli.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gfpjlqfso.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gvcxrngtv.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gtuktlecn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gpswgpvjj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gosxdehys.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/grjgbxusi.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/grwozdiph.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcbecrqqg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gcvxaanbc.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gxppplffu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gvqtpdcmg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtxuoccou.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gikkuibeh.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gdjlfjrwe.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gnbpxomnd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gutirnbcj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/ggqhwreab.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gnovcjmue.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gnmhcjvhk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/grfrcqtww.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gdublqams.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gapuidmiy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gxmxuvyjk.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gytrdtvvn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gipgkwfps.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmvlketas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/givnmhdfd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/govhhtesy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gwqnyasma.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gxrzywnxz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/ghoumahnd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gpkpmetbc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gfctxznpl.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjqaaijwz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/grybuohem.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gdpcvdbmj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqcjckjus.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/ggazsefgl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/grpxxpdgn.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gprbffznc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gvelhurxv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gmefrwjxc.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gusocirbx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gzuheodzu.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gttswzcdd.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gmjxovmdv.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/glofvizbg.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glnefldwr.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gpobkzmnt.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvkspfbsg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gtphfpmjj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/ghfohcmoq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gjwzzasfs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzlsygajx.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gprgevcvg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/glwsffrgc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gnbqeplup.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gcoicvzgw.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gjgfexndl.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gzzmjajui.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gxigttxno.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gsxbmhryh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gypfvmvjt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gsjskuobn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gczrunfia.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gqsiijdia.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gdncsrksu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gxobhsxxq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gxbaktwzs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gfhmvilub.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gsefyyazb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpvucnbfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gsbadcblh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gvyhrpbqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gawtdcoyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gzvounrib.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gazgvmpzx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gbyklhjnh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gptntwcax.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gvwlqccgy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gwdynreao.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gullgvhgu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmqrvwybz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gsdnulbck.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gnpqioxjz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gbsxzeqha.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/ggkgmfabl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gwuenbnjb.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghysuwdkw.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/getbzrpxq.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/goyoyuwjm.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gjqkzayms.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gaoicegpm.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbyckleuy.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaavfomm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmqssqhld.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gxcxaefnw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggfqzsjyx.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghzvalfag.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gedwwtzyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gqxdqrbwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gaxhsjklr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/glycvwcvm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gxjjuprbf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/goomlzlpb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gnajudnbg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmrajucwx.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/ggfcjiqdi.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqdcdpuat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gmqzwdfqk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwfswjjby.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/grczljwsw.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjtqhpjya.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/ghinyxsuc.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gdyhgzgkv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gdmzcbgvd.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gnunbztbj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gqjveugqh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gyifdyjut.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/garlqtsen.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gmjvtwtnt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gehbmcriw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gxszhjlyl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gcyubqndl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gmesvrynp.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/genbcjxor.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggtwsekft.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gnuousrng.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/grilzciuh.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gythakaef.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gfgfiijxi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gjfenjkec.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gteujwzbc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpdmrkxxu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gfkjcvpsd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gahhibher.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gcdrbqjch.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyxoidbvh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/grjkhdnws.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ghujytfkz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gvgxrvsxs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gagkgbvfh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gjctzhzpp.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gxpuhnarz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gzgviawmy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gcfovpmal.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggqreakdp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjelhyees.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggbellwma.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gnnobjiya.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxwclpjtl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gustmabzx.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/ghbrgltjq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gxzvvpboc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/guurdhrtl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzdxkoqzq.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gmpeyxbsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/grcogtnyy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkmnywfxv.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gdinkwvfv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gicjwglnp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gpopqsrvx.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/geviqisob.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gylcsgzxx.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggaivfqaf.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/govuamvrt.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gygtrpsnx.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gyyntnlwx.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gxixdrxgp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gqdlnrzoj.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gtjryacbw.sHtML


<!-- 参考信息 -->