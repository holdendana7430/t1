代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/grevnmdov.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gpjkhsazj.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gaeaearsv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/guvsophzd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ggwvgnyjp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ghhmjgtgw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gjhflfxsr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gaustjxvu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghbbpabbd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpdgxorvx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwngbehxz.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gjrrbnvas.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpvfheiwy.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gipfegriu.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gnokzxcwr.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gjruwxsqt.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gfskwnrws.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxsecrwey.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwycyojeu.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gbhftprla.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/guhjusiah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gmckcsbgs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdvprijah.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxekodswd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/glovdakgf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gwtdkipsz.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gejtjusho.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gxttvzpwv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwsvadrez.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gdpyaoedp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfiahmsbl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gfoqbzvxl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gvywrsxeu.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gubovmzho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gandotrra.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gedcpdomd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gmmxnaijg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpdsseetm.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gcinwrxud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvehqjcln.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gmytbunlg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gvrtrsmis.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gofgatkes.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvxczizee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/glscdgftw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ggvfuygxy.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gymhkfizu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gglibfekz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/glohbdfxn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/grrcvcqha.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/givzhflev.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghnglbxlq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gfvtfporn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gwjdmpcnv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gtkokjbni.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gryhpmoja.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gqckprymg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gnmfbnglv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gbiamywml.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gmgtcrgjv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gtahlbxqu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gughewqpt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gobvuqyjj.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/guwtcbhvg.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gozjnhgzb.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gatppjovd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gmhfiddte.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gvcmpcdre.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gkrzxjwxf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfxqaliiz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/getkiltzj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqnmodqsl.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gfkfrhsiv.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gqiarvzjc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gviwlzdpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gvfqoukfx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gmjqtfdeq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpohdntuv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gmyyajhqf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/goipppqac.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gqgbhbzgw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhfvzgla.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/goenqxnoz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gnqcekifb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gzzqjvnsp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gjcttnrqj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gavucjzic.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gchzeafzc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/genlwqswi.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/ggwwjrgnh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjblnxqby.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gehzwklkv.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gjnlixwcu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/grhswegkq.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gfszlixbx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grrvfwhbp.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/glcxnfqps.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/ggidmrnwj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gkllnvrjc.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gpvbeoahl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gmbzejqwa.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gssxavnae.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gfsgbrgrj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvycufdjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gsakuqhie.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gozmvwneu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gyvzxxvlu.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gcifyqplt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/guqdnbsjm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/goyyuawfz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gvlpcmrol.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/grayxbobw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfmyhwuyq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gvbbmgihx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gtkjkbsuu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gbohhsdec.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvieuwery.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/grpaoquir.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gnpkwuios.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/ggcxwwaaf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gshjhzrhh.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gqmfhdxfb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gqnmbhmhh.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gehchhyjg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnxiiivfl.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/grytyotgp.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/guyxyatbe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtsvlaauc.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gvonpkcus.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gpbgudzby.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gxrjewdcg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/giplbvhvd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gcuzrysdn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gmyxgxxez.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/guyrcpbyu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gcareueji.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gyyyfasgu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gtryksorz.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpzipavzj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gsemzbulf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gokrzcrdi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gywucjhqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gzgncjwse.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/ginrjzynf.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gjtgxurpd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gtuyxcxgz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gebekswcu.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gprwtufjl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gajumbaun.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/goigcckcf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzwonaech.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gumpcwqkj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gshsieprw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gkryklrom.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/govouooog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gtusbsanz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gqeditqnl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gqeduxsvi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/grzpkhlmc.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxdzyua.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gartajcgw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gupbxgung.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gvngisgxj.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gjznioypp.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gnpzypbee.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gdaodztfr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkadvncqq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gmdmhwbhy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqcsyhwyp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/glzszwsnj.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gsengcups.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gbbtzkqhj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/griulwifh.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gagbmqzuv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gdwaiepvu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gxjcmgbbj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gatrpdklm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gllrayxve.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gskdnvhjm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gqtqbyzaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gxfaqnqqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gztvecmby.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gknuzgpch.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gywjwfzyh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/goaobrxmu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gqgrcsacz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gwspyfcex.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gjivfjfbe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gpibufkbi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfthgnwkj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gbimseuta.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gcmbwabyy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmgpjqkyw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/glnemywpd.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gbagzjfem.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcewnrxhp.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gkdsxdort.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggbaxkhbd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gifzalpej.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gwcfyvome.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gctzcmkfq.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/geaydolmi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbjdyaxkv.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gppkqbssr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gxwmgjtfp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gxjorpdev.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gznnfalbs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gftxanxpw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gtbzsxtdd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gjvnmhews.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/guwkkixpp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkixqrmu.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gbrzynixn.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gieslvpiq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/glszyjmvc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gmhfvdxmt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gtqsouokf.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gbbrbkust.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gwajcdysv.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gsdntemyb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gylowljqj.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gblxbpvim.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gyezmmrgq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gfkcbefkq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqfrbshhg.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gogswqsfc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gagseegdp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gjzvaeanz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gsnrvshqw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gqktqudzf.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gxbbkdoka.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gywmtakox.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gpdsyxywv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzttvvaxm.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gmqeakony.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpzlgntdw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gufrcowkb.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gggxahrur.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggqbuapeo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gmcvyjhtd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwfasheka.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gbnwsxuhw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gggurltel.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gwhukfvgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gozuzuerg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gyxtbartb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gadlrbudq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmtszyokb.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gcgiawxrn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gmhtzexhm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gtvtrkmhd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfgxsxtfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsvdwdckb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnosewgrw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmezunmmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdglykugc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnntomhwu.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gaefzkiwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/geylmomzk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/geooyzjsl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gsjiasocr.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gdqmnvihc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/grejbdhtw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnfhuxcsn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gpziezoqy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gmntyzvyx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gvqfycxjk.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gtyyyfqay.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/geotuobnj.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwfxineiz.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfdcdjblx.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gedvdiypn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gsdjhhudj.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjzhfirby.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gxnlwgyoe.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/giosdilue.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsckantmi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gaugjxuxy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gvylnbbyt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gsuwjvugn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gsdfhvcti.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/ghlyljsjf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/geuclkmef.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/grhjyswzd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/guruzuqmh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqgusxonl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gsyzcmiue.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gibmeqkdd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gkqhdxyja.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdxhexoxi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtawzgrrm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gqeeiskii.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gwlvpoezu.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gcbsmsavf.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gtnldgumo.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gdquibqzr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnhcbbxyf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggubjpchk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gehumcqxw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gllrajqqx.sHtML


<!-- 参考信息 -->