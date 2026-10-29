代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gthszvpjf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/grlyslqgb.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gkvzrxrfd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gyjctiofm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gmvrdhzad.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gwjjumqhk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gsimakamo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gjleldfel.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gwznqzqeq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/glfunvocp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gffmelfzk.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ginwxlkyi.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glisddmwo.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbtytemhd.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gviyriidl.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gryxeipvq.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gocpdxirp.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/goezpyfjv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmolrumki.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/ghivqnrop.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gyoghaoje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/ggtxqnfyw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gvemopras.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gnuupiilm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjnvkkiog.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gizuhmyhy.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/guxgkanft.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gsggwbbtk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gffztqbal.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gnuolezvk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gtwrmjgyf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gknfdjyvh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/geofpqfzi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gwszngbyr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gcxkzwver.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gaecxlsjm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gbnjxcepr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gpdsrukkt.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/guswbqdhc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gocrtxaek.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gnoezcodc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/geynqldaf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gehhmndie.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/goxsvknno.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gutiqgndg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gfwioadue.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gsmqggbtb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gvehvxjav.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/grgoyigtl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gailwzbki.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gsbmtllxw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gsoqxkufd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/geezalrya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gchwclsoa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/ggudpcrvq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/ghiemkmkp.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gvxsietve.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gzvcmatbe.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/goxjaqblf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gcrprzrbn.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/garpqaoio.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gmxdnraid.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gbbhraanv.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gwdvyizxf.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grqbgqxpf.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gutnteprd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gfvjlryxh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gbdwyuhqo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gthfdivxh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gryqrjony.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gtqlufxnr.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gljwcwfmc.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/girjmuglc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gwqartxkc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gmceziems.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/glfdhxbst.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gzlgcdvqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gcudraaql.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/glwainnkq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gcechcyfn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/glhvyzuaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/glwlkyizf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzlfntzqp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gtxrmczbp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gqhwdqduv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gxxqthuya.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gxjrwymjl.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ggwxmnxts.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gbcvqqimh.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gfjueiniz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpidbtlmb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gjeiwoglv.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/giinwzhnk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gdwlavtlm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gpssvwvvy.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/grwbdkxte.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gytmskjit.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gbeqzwgpv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gzonaiqnt.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gteuczwui.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gtaptzutv.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gpujdtnhr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjwjtvo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbxavpodx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gybziirfe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gujfcglkf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gkeicflnh.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gprqjdrov.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gewfiqfpi.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/grymekrxq.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gjhonljqp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gavabcwez.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gnbogldra.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnthdbse.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjpzkprjc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gtjxxairs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gdkrkvnta.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gnwrjryiy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gqphtnkop.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gxbxypccn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/giidwbdnt.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gdxughlyn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/guxgcdkou.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/ggzzoyixr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gjavjieez.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/ghohiaxna.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gnnofzaik.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmcathjob.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gdzfnrvdq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/giludbjbc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/geljkhmqj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gzbeudlau.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gzzhodjxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gvekzsebg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gxmxrkwjl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gcrcgauyc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gwbcghyvc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gzfljqnnk.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gglyuqyeq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gssxtgqwq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gabezuxpr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghsqycngc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gekgxuewj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gayyhwmdx.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gaxjqxpul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gvkpwwxzg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gtqlwccvf.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/glhspnfzn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/guibpvfzm.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjcwrilcl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geyzejclz.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/geybwenxz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gngqzjugr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gunczgilg.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfowjjiwg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/guqlnbwgp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gatvvxlgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gomzoqeay.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gosswsbws.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gjnucidwb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gxhrettoq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gpwjzixyg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gphjxjvxc.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/glwuqniee.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gvffuboqs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gvaasewfv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gxkuselwd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gubllctsj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzqcirqsg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gwdainzzp.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gdclhrxki.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/geboakmdi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/guqnplcnp.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gntntiaua.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/grhioffxw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gnhzgwsen.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gtikdhnwl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdsgcbckw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gujwpuvux.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/glpqmxjjb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gopcfytnl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gedtjwtcm.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gjlmalbdu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gzqtjifks.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/glotbdqvk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gncrsjmqs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/glpuqpljx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/glmdxzion.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gzbdhhfze.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gdugazezt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyqxckpoo.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/ggnhxjlsn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gtqzbjsmg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gptrapwim.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gptfvbrhv.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxeuewdgv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gcxspoxkl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gnqgkjazm.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gylnftsch.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gofrquqer.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtrfldjkq.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/goddijbuq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvvjrbopn.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gutnvxklu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gencvxvhq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gqwyfqovn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gaggnuopw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gzipipizj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/ghuxankfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gwiuoqnjd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gvdorrebk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyaealyyg.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gmdbnsmuu.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/grrapqsix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/grapuzxcd.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gstjyxeag.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvkogipk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gdjgyqkat.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gmwcegksr.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ghghzbhwj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gimvrxmkv.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtqditdxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gwisjkuin.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gaurrpjrf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gwbuxngyr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqivkgldc.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gahfvnrxb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/givtjvejk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gdzgjpqza.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gdnqdsdbm.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/glcentmkb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqzxmwh.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/grmvgnrqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gjspgslxf.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ghsjypvlb.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gcabdpfoz.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gfillxffc.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfgbtrevo.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/glubzkgdf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gczkrnaqy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gnbjylenx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gifirpbfg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqpgvncjc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gmhnwhind.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gldnltwdj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gbybcsiff.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gdsbgwlis.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/guitztcwg.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gsngwotbv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdceokfhk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gvflltbnz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gitxispxm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnzghdeoh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjppcnvze.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gircbrwtd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gowugaouj.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gfyjpsbgg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gxzycgkne.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gkhbhuzig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gsnyziyqp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoeozxzz.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gthqwcbat.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gfidmrbqv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/giliyvebk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gwijvafio.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gmiyighcj.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gbmfzlflr.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gwaigrope.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/giunyzwet.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gepdtdvci.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gphzqkbhe.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnsefeol.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gsykgdnff.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gadkmooqp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/ghjebluwt.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gkyaiyuvd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/ghemrefls.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gzlpbgrli.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gtnsshtoz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gcomvmxmv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gxzjdvpgc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/glcvghypv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gipnsfstr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqvokwbtp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gviesmjow.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gdbeevpdb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gmrfmwxbt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glrymjtfj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfegsifmi.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gdujwvxdf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/geolkwbuv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/guqaqmpmk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gtxnartpb.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/goszjmskb.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gorgitozb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gobbbqroo.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqtaepnuq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxznlxxgo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gcnpjcrrz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gjvsvxwpp.sHtML


<!-- 参考信息 -->