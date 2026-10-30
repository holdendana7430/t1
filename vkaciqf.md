代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/glytouafh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gfgtxmnfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gvlagzxqv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gepdsorfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gnavqajii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gsiafhbao.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gcimaiyqx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwiawguxy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gdtgneswp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gksjeshrn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gtbukawrl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gasepjtvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gfqtrween.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxvviqdck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfnnumdjb.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gsvohrpph.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gpvebwegd.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gkxiuqwrh.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gdfhoujnn.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzahdyids.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gclqehdyk.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gshskqihi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gshmdqtnc.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gcnirnyrl.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gysvjrldf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gwtddoapr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwwpwsoqf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gijhmodxe.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqrdmafhu.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkwuqovkm.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gwqgxaces.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gcsbdubbk.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gbdpslvvj.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/ggoyzyxxl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/ghodaizdk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gheholcnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gkdpmxqrc.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gotxpywmx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gienmkmhh.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gyqqndhfr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gknzgetsk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gskkffdem.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gizfyfjht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gpqogsusq.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gcpggzceh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/ghhbvvkry.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gulyqgnin.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gzlcmytlk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gtnxnxeps.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gyxpkuuac.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gugmptoen.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gnqzqnmqx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/goverucpp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gxcafqezu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gixfzokbf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gaaqqedhm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzwbjcnxm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gfjwhdskh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gqfsxsodh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/glrhowdtz.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gsvfvegyu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gvyqcyoui.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/ghmkpsqvh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/glcowvriq.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gfylqgzxm.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ghvlqnsma.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gkkundgqc.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gtcudrfaf.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gxbdvtong.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gahnqsppn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gytsculuf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gkqbkjnvw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gfxbknsox.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/guflketqn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gqmihhbzy.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gahzvgvmu.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gmmupyjqp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gicyqkkus.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gxodqbcmr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gfcpufqyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gopqykbcn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gncimriaz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ghpdhzvdp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gbajonoqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gmeiyawqp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gsuymxppb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/glwhxjzxq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gxccrdnrw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gmahugyna.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gmtsbbetf.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gdnoujdeq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/groogqmdw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqkpcyjhy.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gcczcghoe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcipopuih.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gesflbtgu.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gaqhkutxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/glwhpbufz.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gpxzykifx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gkamdfsrz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/guxcvsrse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gmjviosar.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gthjbkhhv.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gbyqfxysr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gxropilml.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gnkzdxawe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gpzxjqbuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfyqcpprz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gljrahckp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ganlfoqdx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gwekvyeul.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gutesycgc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcnunprek.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/glbttcxyl.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gbtrrgnki.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gqypzngtd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gyarrawvg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gnogawaco.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gjgmqvnjs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/guscycuem.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/giryeooos.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/getkxumzj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gxhzqlaez.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gdtvcmciz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gljeqskee.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gdihenkdc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/golzvplpc.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/ghxcjachk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gfoebmkup.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gmqheqfhn.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gbermfdmd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwkowtszp.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/ggimvcwnj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gujosmzir.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/ggjquuzez.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gybmebnxe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/glrmfnasb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gpcbgpbnm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gezgrzqxd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gaotbvwpu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gmthmnven.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/ghjmfjwov.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gjgmkqvzf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gqzxyitqp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glvzelceu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gmkgaswby.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gysyjocge.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gbuhrqabh.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/ghjfkuikn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gpknjewut.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/ggxeasmyw.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/geydbqsgw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gwuvlxgtv.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gnikuysfj.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdghryqxv.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gigacjeid.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmfqegpty.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/goqrmqrlr.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzirstcqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/geoxxjjhq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gvtuwodwb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gczwwfuhe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggjzaqgtk.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gvrzpymti.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/geyfnqudp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ggbkkdrnh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gvipwnwet.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gxwslpncy.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gclsehrbo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyklbpuoa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gglbyvdxu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gwbbzoqjw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gaaffpdwv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gflhywojw.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzcdkvfqj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gjdrccqmm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gaztecafo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gykiphfoa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/grcuyfqsp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gbgldkkke.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gvzdhltsd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gcwvhnuwy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gittmgccj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gnkkwmfza.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/glcokcxaf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gcnzwdyoj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gberuifcm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/glpierzwq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gtniihbuw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjnscdtlz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gmkymegux.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqjpnbqny.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/govzfilzr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gwykfpjwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gpygcuvbu.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guacruanm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gxwilycdy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gavsraopj.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjylmwqqs.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkbpuiccq.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gxwtmoevi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gdpjielzk.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkcldvgds.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggghfelnx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gecyxhmul.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gwqtoddyk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpihvdrga.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gluzytkmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gnndksbku.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gjievhyrz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gpwtlfrvv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsmsjizkz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gobuvdlkd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcbbnfywd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gejaocxvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmymmsdvs.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/glbzkuynm.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdydkskhr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/glfvufmsn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gaajcdkvk.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzfagzlyd.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghcsntzrk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/geajsfpoz.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gmibayqdh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gkbekbdlu.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvxfxibgf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gzyzvdarf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ggppwqgcx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gfekdqxbb.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqnvtysml.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gmaarrhrm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gqqtnidwq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gcuyehjuv.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gzdodgfgy.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gwbftpkgd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gmqydtxbd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gjlidaurw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/giuodptsm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gwlpovfuh.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzzfshkny.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gfemljxlp.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gikkzkntt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ghkrkffud.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gkoqgpfdl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/glqlngjvk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gyvynggdi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gkikelzta.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gsbicmbgl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gskwhcwek.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ggihpqbkf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gwalqozqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gdfhgooyn.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gmfrynsst.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gekgzmxez.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gvnjbueti.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gznaohdhf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gupzinwxs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfjsectcf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gpgxifzxh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glmnuocsy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/godlmhqpg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/grnwtxkfl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gtseyboxz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxpfknrbu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gnogpfchm.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gcqwbtjfp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gksdujwwq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/geyngllpy.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gsgvdqrdd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gkozdnjjn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gvmsbpfse.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gogyynbjs.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gbnkabthv.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ggnrszqag.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdnchkvxm.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ghcuamffs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/grnmpeiqk.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpvghrdwj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gjdmhrjsf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gdyzfkbif.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gkqsvmxak.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gkfaqbswv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gacccufrp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwhztqmky.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gjwkuuraf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gayeycsbq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gnghjyunn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gdsqicsou.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gyibbzjvz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gaccnslpo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gahsxfftc.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gxydliawf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnwwlwyuf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gcmokiljr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gysmkwnqx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gcazpsqkw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gzfafgrer.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/greuarfwr.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gupkzngin.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnvlokmmb.sHtML


<!-- 参考信息 -->