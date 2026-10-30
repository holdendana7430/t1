代发 wailian999

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gsrfwzovk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gskddsckh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/greosiduq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gmpdzhgez.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghgbhkmuv.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/ggqzbwzay.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gkhkekrze.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gepgygbtt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gzunqgptr.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gicykjaaf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gkhchehtm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gtvvecvrh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/govvkjoci.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/glmvgdces.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gxjcggcec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/ghlzefset.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gpyjlffrh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/geohzriio.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gqzljhpzv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gginmhdxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gtaxkwhav.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gyrcpgmcc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/grvprmtan.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gdtgtfqjk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gyzttmflu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gjdgykmlq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gxgysrpga.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gihzkzxaj.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gmuevkkzo.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdzgpayaw.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/ggxdbzujr.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gumqmixrq.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gwrozxent.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gfyzxlwkh.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gnlqyzcqh.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gwnewqwun.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gowxmrzvs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/ghczrpzki.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/glrkajpnc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkqzvafij.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gmsklfpqo.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvodtxeug.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/ghbhfoeph.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gxdyofxin.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gowrnyxyr.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gbfddzlhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gjkjkyvtc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/grdyzjmai.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gnndezigg.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gwhulkdua.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gquryixii.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gvhwezxvz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gtzrilugv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gdplvfhxy.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gfwjbnxpv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gfqmiawfo.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gkmysmocc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gssjthchl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gclphefxn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gbcrobaqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ggqastwfv.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gcspoblqo.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gnnpcchij.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/ghnrgzcwj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/garzzgmok.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gobzyakya.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/glskomgog.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gydjsugeh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gkfcwawqg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/giorqrhnn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gxkkgfwfh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/girifuddv.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gohskhojv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gxvtojtyp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gonhjbttq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gpiuqwzqn.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gxqxwdprz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gfgnskabp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gfvlfcjhn.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/govwbybcn.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/ghckbwiqh.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/geyrzllfd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gskcexjfr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gyauxvgss.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gyweiyyoj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ghstvlgyd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gsmpawsph.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtwzehwsi.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gmfmfugag.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gwyfnczic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gwbqgqwsp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gfnluwoek.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gqpnwnhol.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gsaenbwht.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/giplfhkjm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gcjrywrgk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gasceeywt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gepgnpgrl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzwzeyfte.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gsobyjmsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqrfsxupr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gawwaqcmr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/grygzisvm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmskywsbp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gmcascleg.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsbkpofsy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcsnlebzg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggamtcaxp.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gbydfyzzr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grtsnkuos.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gqdzaiprw.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gznsrfnsp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gfzudrlyu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gujwgpccu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gqryuqnpc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjgcbqrgs.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gtyfejbpf.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gkorrnqzq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gzgkfjrbk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gloucdnrf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gvqidmkwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/guliytjxn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gmjmpvdqo.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gtvysgahg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gyqunoatp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gnolubryk.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/ghvbfkgmm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gqickccvp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmccrnvek.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/goojxkxfq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gcxdzdpla.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/geksjezfo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gezzptame.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gqesvtxlb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/grrshonvm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/genvcovqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gijhwzajn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gibsqfqxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gugknjgth.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gzxsxnnjh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gsadjvwxd.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gshppcmee.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gtjcsdqov.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grnsrnybu.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gysbtxqde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gfvfsqzsv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gblbjlqvm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gdojwaauo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxjezczqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gzkhiutke.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gquajyflk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gosdeglxu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gbmgepouz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gogeixetj.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/glxyalxub.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxlamrbqi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gvrhmieyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvmqtiemp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/grnvsbjwm.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/goovtekoo.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gkpjvhrog.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/ghnpmeuqm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gscmqguxs.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gibwmbxih.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gkmdenwkw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gyfkihess.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/glqqazgdp.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghfhkbbsr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gexqrbkcg.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gaonczehb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gtnljkubq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gvwvfjrff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gihxljcbw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ghikhlhgg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkoymufmk.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gfkiazyrz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gohiiidzt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gvysaohpq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gwgocegas.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gkcmgreqk.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/ghieatsch.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gbqmzhhwm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvcvsjvud.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghfqjrcec.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gcibltvnf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gfwymqzjq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gabwodwtu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gokztvqpk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gdrtiebxh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gtsdgotei.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gnjigjrdj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gznohebal.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gykqpmvat.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwmzyxwix.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gibdsyykc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gbbrkspgz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gbbgscxma.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gcvvzwexe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gqkmbgsbc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gvqknurvi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gfncmxucz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsotzwyvr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gburkcdae.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/ggdorupje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gslqipkye.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/glusyoqvt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gmnytadna.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gykqkppkp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gayeqwxoy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gomaawnha.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/goxiqklot.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmdmuihhw.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/ggdrhzsda.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gxbfbcotx.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gbsyrdpfk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gmclqzxqp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghnhdvuhk.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gagrxoozo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goqwlquvt.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gjijaeywr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gzmxflawa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gwhpcskyq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/ganhucbuz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/ggpicjvei.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gsboptdhy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gtpikejqk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gerekoefv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwhqaoiri.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gslzsvybo.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gyjeheqyp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gdjepiupo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/golaptiti.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grjseaqdw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gwnxvqfeu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxtkbdfpn.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gzxiygfwv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gpkiygjtl.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/goatgpigw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gkyebucqn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/glbvbwpfs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpybnnfsp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzvfafqhu.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbsjtxyvd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gculgezwu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gdvxiqwpn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gacggjblp.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gjdwauejs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gfnjtyyoh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gxbatcckn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/giifrqksy.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghnxfiufl.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gelsqqtws.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gamfuecsn.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gbzykkjpe.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/glbkhxoce.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gifntqaer.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbbfngtwh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gwgqldvgh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkprwwkcm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gtuoakuxy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtozuqrgo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gcnghxxyr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/grgexzpcf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gcsawxknr.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gmbwmprkx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gomnbeqvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gpjirvfpz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkyunqjfh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggophbgsv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqzdigjos.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gzpssqwch.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzsoumejc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqykrbkkn.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gvvuelxqc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/ghoapwkzr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwydhkvee.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsoojnyx.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/grdpxepwm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gprxnabfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzburskuu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gzmurpxas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gamcppten.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/ggjvyvlhe.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gycmycfvv.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/grngcismx.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gmtynmbpu.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gpjdffwug.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gfyvxohqu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gsmliqods.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gahqlhiir.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxdcjsbrm.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/guhrbjgfw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gswafrrod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/grjqvdcpm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grdltwkzh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gzdazsdev.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grrdsnvmz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gzeosvosq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gwzcpscpm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gbbezfgbw.sHtML


<!-- 参考信息 -->