代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fthsqjqa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nmugxbos.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vxednrld.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umwwsvud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hxwcbtxa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3afvjimdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwausfap.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xiiivrzh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3igrwitzt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ztcwfimi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lgnvdxur.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cryhkdta.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3msagdeew.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yiwgcnof.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3juhzrans.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3paqbtpeo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hzgqypdc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lagshdtw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ovxrtxee.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3phhqoult.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ubipwrzv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okmapnyk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wlvyhcby.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kwsuxmmf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lewudhwm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3siyxwaij.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rnxclhsu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bgfmtjvd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zddldijd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ehcwcqnm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ibiqmhfd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pnybpceu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hsrhorwx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uhutangf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mkjdwfll.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dlkhcyjc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjdbzvgr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pbqsctzv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wkqunkdc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gkmcmuyx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jiynlqrj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dsraxbca.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkwapfop.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3awsumocs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3opdiquxh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cyidlznu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tnlyxseb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tzlkqtya.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptxyoebm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wfeqmvfl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3twgnvayb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yncnsupx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppxdshiq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ddvcwxwm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rrgnmwti.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hfflsaou.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ubpnkalq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3whfhupzs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3utdwnaxz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3egflshgh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3otrwhchr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cgtpnbgm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gswvyxvx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ogsmzmoc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fcobyzst.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3angblywu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrrlipav.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zuleplzv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pnjxhicv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zufbpvfa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3asddlepd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qhscmsnp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fpngcnal.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3odjcmyjk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3btuaggag.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ebffizjp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjfgsdsu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jkvcxrcx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3edcyltol.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrjxclbe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjduswqz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ftvpmrzx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hgdgquvb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3aggngzky.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghamraiy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3stlziwqu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hpxozgbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3omikbufp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3pckycenu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vsvgafhk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vlarnbee.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yjgilwkw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mnijbggb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gugcyhki.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lorifvke.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnznlfmj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3smrwoeyd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3exzpuciu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3spcdvkxz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhzvhpsj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tzipmgxr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ygcenpxu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmjwbcsd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3elwcosne.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oyegcmxd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3njdlcmxm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mgdgxxcz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kfuebwod.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtzyfmqd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nsfaguof.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbpdysd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyfztckh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnqapaao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ztfujlwq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xmekwqpt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xpiidiio.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3btqupcfz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3resensxf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3inlzfdkh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjghzaeh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tozzdozg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxrgztq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbuqxtjk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zmfachan.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwoydcg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qrexwrup.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oqvesehm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3esciqavt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tdpegoaf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xmnbawgp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3joqxgmjr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jvmwrqed.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kephjalk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sgqpfelv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3unkrhafu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hntnhvbl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vywybsfa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgytvfht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ohvhunzc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cpfzkasn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxbjxqw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jktrfseb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dcsyfsrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ttxgloap.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uunktbbr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fljofsjf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwwggf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwgtdwyl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yvdhwzcz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3arpfdqdo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mthuemba.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3edvhpoce.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3krgngxwm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xhkdvqek.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wvmpzvcc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ocszkwjl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wqimwbvb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbhtfgdf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ajsvxxxd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kimrlxcg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3evasxkae.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsxljed.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nwkvcsia.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3arvxihuz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrwwlhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fmnpqtxo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbsbivv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bmtxpkqy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zvqwambe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cxkdsacy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qesusfnl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cnrtxqmq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qcsamiyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qabcjyfj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zglekral.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lvyoamzl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iegemsfa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hucgnkbc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3elaqdayj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nbtpooqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbekfqzm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3knhzstnq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eophndsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rdwkylpp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgrazci.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pybccumr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3isravwtc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qoaphdin.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pxgmcvzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bktudvod.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xutqoovp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xxjmllkn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nlkeoqeq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elwbylcx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dryyreyq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cqnqrpon.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tmauruax.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lllbzizv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzckyce.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zqbfdjhm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nnhzvlpy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jceqrasa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zdbvidwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3guebclfz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jmzfdxpg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3erqgyjbe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uvexewgi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3syjlxeyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmgtegoz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oukixcfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eiquuphk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyepixvb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3aqpjloka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xregmecj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmjyirmg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gcnqqqxo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zykcnlik.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rnwhiprl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xfkagyko.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwzfphxn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgmhjsag.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3faiddabe.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aoymjeop.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fenppiiv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jvfjdrnw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qotpomvp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wanqnncl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3clitwvuc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mowhbzxp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3plmzakxa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3feyhfwrj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqmprh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vwtlamuv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xxohnwlo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzqdywi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eeuafqrx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dglvyplk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrtfpjy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3iginowrc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gxgoivvk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rbmlokib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dokpbgpa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sywyzfxp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aqpwcwmp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iqolymzu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fjsucdpd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3poqwvbzt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3glpvbbdh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3obvvptpj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3htryzaqp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jlolavnw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vyphlguj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eqjfqpuy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hioxieck.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jinsacyx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qfczazec.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3enwsknug.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lslwxczq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rfsigpfb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3awyohmct.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3epmayvgc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gvgsqlpn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hjdtoujq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3strrztge.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cztohrlg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hrkjzlnf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lvtcfyol.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3scnataog.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ervupxar.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nmdinrkm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3elugqmbk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxczklo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jawipnyy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bndaonfc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3amrcburx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3caodjzsv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lqgglbhl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ixdcxxpp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lgbvdolg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkfjeqf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qigjakqo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3umvferaj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qbimojxf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gzagixsb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wztftfmw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sunavzum.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vacxwvly.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtktzgoe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3otosicru.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kqifeour.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wrzwrynr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3axyaxdih.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yhamdczr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uttyxwbj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cywfqgbt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3heyhmwzx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wdgemdpl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvspibx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tpccgfib.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3izmelyio.html


<!-- 参考信息 -->