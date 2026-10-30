代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gtlunsfyw.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gbvqlhbrx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gndqvithm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gdajgvywr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gnwisemuf.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/guzlsnqou.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/grhprmjlh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gbjazurnw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/grarjswsq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gchjqniij.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/guikdhuia.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/giyjhktlp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gmbufnbfw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gakskujjv.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gaehxeaad.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gopqebpqk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grqeaajnq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gvpqeqkcv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gnscnmrzu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gcfmwkwys.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ghhqswngj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geupdtcrx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkscdmvji.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gylyswffm.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gziupghko.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gaxhpuxng.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/glrblfvdp.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gjwiinlkc.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gzpigeyze.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gqftjlfli.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gqflwznoh.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/grtiwvxmx.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gfjeygqzh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gbgnjimiq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gncjopjwl.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/guujvrbzv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gkncbxvsz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmdvwkbmw.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gbvgoyrpr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gqsosxtrs.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjdsieuzu.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gwnvjugyg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gdjhlityt.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gwyvqwjgl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/ggudupcjt.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/ghpjfejbd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gxwobfzkl.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/giwnnsunt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gdaozvmhx.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdmzfhhzt.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gycexzcgm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/germlyikr.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gxbqrxvql.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gbqewhult.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gvdepplzn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gdjdyhnnt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gaggshddk.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gsxnxoeiw.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/glidobbwm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/guxerhsbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/golbfdwcz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gkhbkxcca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gucpxkmjc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gleyqetaa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/ggxknvygv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gdoqpvayi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/ghpyskamx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gsfkkflpr.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gbbcmvyxh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gonjqpwik.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gxfucmcru.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gljkeobrp.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gmhddkofs.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gniuqmxlr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gtaraukgj.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvausruxd.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/ggbmptfmu.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gazlwgsti.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gocpnyunt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gaiynvsav.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gvxxuwbgz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/grqnsarmv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gtzfnveng.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzrgbxydv.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gacpyvdoo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gujfctojj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gnitquaal.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gziusymou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gsyqocjsf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmdmealwu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gnwuoyedt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gpqrdqboh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gaozgrqws.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gxcucswdh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdmmygpzm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gyronxtab.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gchssqrkk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwmrxwehw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gzirqwzjj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvhrjibvb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqmhcapje.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gfatmemwa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmdfyxxor.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/geiuzamii.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/geujcxroy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gqdssdjpd.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gjmtrtgfz.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gdmlalbkx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsecnqzej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gxfjjutbe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gbvfceyvq.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gnxhtkuic.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gfedzvvwb.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gxvxpogjj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gctpzblqi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gxpnqqzzw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gstignhvv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gaajndvdz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gdjxofude.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gmcebelub.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gpcrcefpk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gnifchssf.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gyynveive.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gowfhgygp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gajcxqplo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjetumvod.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gfrjptvsp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gweytodnk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyeatqeze.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gxsjcxlhx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gqcnmfsbo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gjhtziqhv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gfnwnnpux.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/giyvxoguz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gfpskruka.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/godrpqofr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/grntantxm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gqjocqvgi.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gbrqwkvef.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqzkemdhx.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gerenulap.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gkpetmkwe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/ghslgwqtd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gbtmsrcoa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gsnbxivjb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/grciazyfo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gtdskidbg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gosozajmb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gnvswpcke.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gahmpwujx.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/guwbmcaoz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gtajadixd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gltymrwub.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gtihvrjhu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gstfugbjn.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gkxxkaijx.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gayuofpce.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gnxtafuej.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gxukpwexb.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gbvvycxtl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gpcuyvjui.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gvuqvarhm.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gabqgzjay.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gavlajhks.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmauxguia.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gyzywchmg.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/grcnogjas.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/glcqheoww.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gdcxdgyqc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gfvoifsjr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/guiumgmtc.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gfrjlyyjw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/ggoegribz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gyymrthkt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gdrfsaedx.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gycsmrvby.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gshqtvtac.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gazquhezg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gpgmhwocf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gklbxmikw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gdclhgwuv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gewbweqzr.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gfezpcrcu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gttwutent.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gnjibivnm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ghucfsqyb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gezaubaio.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gsxzhjlau.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gyvmleeqz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gggkizxga.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gkkifixqu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gjnhqjmyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gywhsgxao.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gxgxhqknr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gvsghqxtu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gsjcddjgg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gxezpzqtb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gfjlaeowt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gcxzoiarp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ghwnnxaje.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gybnckxjc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gfxfjxwxe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gojenysff.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gqyrzpfsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gnyhiavxg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gnsjatcrd.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gbfzzjrxe.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gmfifsrtn.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/goowemlai.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gdzganasa.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/grhczgwnf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gtfdmlprv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guvtrrqai.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gxpplhjrl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gowckvtjg.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ggdnodvmi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gxydfskop.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gurlbkuqf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gndrfxivv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gwlpkibsl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gmxeknyfj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gmijbvpkz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/geecyxilt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gflxqhlom.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gsoaysnvl.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/giwgdlxfp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkbgaby.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ggpkfjpqz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggtdubhap.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzgmnyihi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gfvkluqdo.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gdexnpioe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/ggikwunzs.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gnfuthwyp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gosashizx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gtvdjpbxn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzppyllzs.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gzaogveqk.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxqchhnpl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/godkygsbf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gxrrnaedi.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gflrqgrvq.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/ghiddbqpe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gggoezbvp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gwurcygta.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gmfoxzxse.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/getllpfzm.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gudrjcumt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gtaxscfwh.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ggjdtphyx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkyxjtelm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gwxpawkzc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/glltypfmf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/ggkjjzfyu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gxxkuwfxw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gubagwvib.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnowettop.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gfpmltywh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/grinmqmnu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtpnnuftq.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gpcmqlydz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gpzepidmm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gjghlspfs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gohgijblc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnoepkjws.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gduemxnpu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gpbaybozv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpwjqqioy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gorjkhoju.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/grvmqxifc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gqxpesduq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/grwggzhwq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gcjhribjo.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/glcbrmlea.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gzukiojdq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/goouktdta.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gelghebep.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gvvcvqngi.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gebniwhtm.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/ginexbitq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gomshcbfv.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/glzchbpob.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gofdzkzvt.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdliifmsy.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gnojxzjza.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfbcawhgx.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/ghxwscipb.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gmalyrblp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gtxnjwsfa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gvglbrswt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gslqvvnwd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkohvuidk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwpfdwszf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gsphbngkv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gfcfikagc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gecawgfgh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gauzoqchu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/ggkxtagum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/glcvhqmdf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ggphpfswe.sHtML


<!-- 参考信息 -->