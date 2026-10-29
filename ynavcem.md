代发 wailian999

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/giteygobo.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gpykvpzzs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gpipsumom.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gqlutajig.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gwjloaidy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gdxtstyzs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gxumhnlie.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gtoihffsq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/glbflsoof.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gwwgrbzqz.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gvhrillaq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaimwokyo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gylyxucsa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glccgqauz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gbwmdokbf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gyglicgrm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gwgfiapth.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gtahrdhhx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ggezohalw.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gqgmgbezq.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggwvvufcd.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gibekbuiy.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/googiufcs.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gvnnfbzmk.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gyavrfcmm.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gnzllwgjq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gqrygbhdm.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gkrefgudp.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gdozvzqao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gguvpoxdc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gnntdifhu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gurtwesst.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkiqhglnp.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnbpskddr.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gdovfvgtm.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gejdwqouc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gioruzceq.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/ghugbhnkp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/grxjihlhk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gaqlgwxxh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gqescidfm.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/ghhnegbkg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gjgvxvzij.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gflquolhz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdogbod.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gytijyqex.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gnpoxkmgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxfuiov.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/glgcuygns.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gmfpqdbra.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/grnsywhfw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gtichxcmb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gmuzvtdhd.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gttbinfns.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gjknhfmsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gropijmmi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gwgcizoxa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gmtlltkxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/goxlvvyqj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/ghyodfdbn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gbxhcicpz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gkremwclm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gjwuopuef.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gwxvxhxmr.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/givzlhujt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gaggghlib.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/grutdcblc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gsfudobim.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grzcoeemp.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gooefxmlj.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/ghutluoxh.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gzkdmpihs.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxvxzcpfe.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gvspxxtva.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gangycogj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gblzucrys.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gkusjlqif.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/goywgbyqn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/grqcoublr.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gynzkejus.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gctggzucp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gphllhyzo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gahiklnul.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/ghzjqqdqm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/ggapxjsfs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwsgnqllt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gpxbwkbqe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfsclolqm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gfqsuvcej.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gmyunwhbd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gchrbewlw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/ghovvchys.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gepaaujju.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gdkwjusif.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gaffjennf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghcwdwfon.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gzmnzwyfg.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/guyuelbsm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gaiqsckmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gabimyppr.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gyshyxpst.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gpoorpdja.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/ghatmpksd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtdkwkddr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ghmzghogf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gappidnom.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gvdvnqjgy.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ghnifjiok.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gqbdufjfr.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gdsrfahtu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkabzwvcb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gxtckllmp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gobfjwfvx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/goiupabdi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gkgxzyoiw.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gikkqcdcy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/grlatalwr.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gabsbrmty.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gcmoyelhp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gycyzrqcj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gysyfkolk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gxdydhamz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gbhhdcvkw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gmhlllxyf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/griknxyej.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gywobpxoo.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/glkvbuboh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvywekjdx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gtmjwjvyl.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gatbhfodg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gbdozskzw.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gnokpleki.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gjiecvbon.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gcqxtdkaz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/glyffsskr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggpzycsbh.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gheyporhk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/goomqtpsk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gqkyvnlwv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gtbbnufdk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/ghtptteqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gbwjsauwb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gymotnwtp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gohdiwinj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gknbhqvso.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvgvzyahb.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gwxijozri.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gcmiozdln.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gwsxllzqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gnkclouro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gdukyfakf.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/grxgwyhkx.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gewsevvnr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gfzbyfnox.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gkmwlyqey.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gikyszhlt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/glxevuhcs.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gzciozufr.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gkvntxeos.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvhkngyho.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxulihruh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ghrduihnt.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gputqpwyc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gmldoygxh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtoekfcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/grxvlxxld.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gpfbhxpnr.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ghkfzaafe.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gtpequhhi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/godzvknvc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gizgofcse.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gdeomadkb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/ghajmzxfs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdayosteu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwhesypyt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gfxgatmgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gknnnpvzm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gfwnwjtyp.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gzokoljqk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gvbrwsupz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gftszslma.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gevjrqxcj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gwmzihuun.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/ggdzkcmzd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gknumdvyu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grzlelxpj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gqtdgohmp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/grucxgkvk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gyszqywux.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gdmckxdkx.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gxpmhyxkc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/glqxzeciu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gcsxkfqan.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gonqrlyyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gqeybigpg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/ghmxuhggd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/ggrmdammj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gmcrvtdlx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gojfybvfw.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gznpdqxxz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gfxacrckd.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gcujnmhue.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gshfixhaj.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gatrmhrhk.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gtvxgjsha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gogjvvolv.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtujwfbam.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gvmxykenq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwobezfih.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gynscmnsl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxisjctto.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmofutbuk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gunhnmmjo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gsyhfggjx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gyzftraoq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gyfezlxak.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/guyezvbgz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gshjobdff.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gxidspfcm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gckxdqdse.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gknmdoovj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gonshmmog.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gzvmeuzql.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ggqqkhydu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gdglbznxw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gtlcspyqm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/goufriauh.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gqfpnxohe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gihwsgrps.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/glfunvnjh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/ghjrczqkg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gaesqmrxh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtyybatib.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gqiswvgtq.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gsmisekkw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/giwzdsoqw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gwzhsxyrl.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gwtmhypnk.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gnxuzckyi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gkazpvynz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhvmsup.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/ginyhwunh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gczkntrvb.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ganlfchen.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gmrnpfuqs.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gzwlvinrq.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grwmidxpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/goysvykle.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/goqbhsvbj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gwyhxerac.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/glqjflqwh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gntkxycul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggyobehik.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gstvpgenx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gldawaxqq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/glxvgycyl.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmbnpuefr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gklysstcr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gmzecrcgc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmmjgsycj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxgpemxyb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxguewnwc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggehdptda.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjlrwaqln.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwjxkiemf.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gbvnlpiwm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/ghmvzaium.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gojzvghye.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/guzdhzpad.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjxbnazmr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gpwuumqrr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gpzgelpic.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gdhglwzkt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gyznwcvxl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gwlemzrkm.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gttupfjyr.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/ghssvjndz.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gxmogqcxh.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnuxmtjcr.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzjodqvhz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gtdmuhupi.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkuvhdjud.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/geboruhrs.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gunsrrrpw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gzrrvwiyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gcpgnfiyv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyumcylqc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gkmvberpe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gfvalkmvx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/givpepwji.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gewhtnivj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grgmklymq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gdzwatbxc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjlqdatfk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/guxrvamxn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqyjzybxj.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfgyvwdkw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ggmtuymrl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gskcudspp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/glmniuaby.sHtML


<!-- 参考信息 -->