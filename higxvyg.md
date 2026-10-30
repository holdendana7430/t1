代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gluxiponm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gyvvpfnld.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gjffvoegp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gqaqgokjp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkhyvhnme.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gdbveepna.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gamoxavtc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gyqhagcob.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gsmwrjvqt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gpoupbuwr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/goaaogpas.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/glovfqzay.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gzvdidxsz.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gfnvgamnb.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gabdiohrs.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzjufvuvx.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gueogovmp.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpiohpieo.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gbmyeuphu.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gvzagpube.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gwwkdmcsv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gegszosnm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gicdlcxls.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghqazxnxh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gvmgcktun.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gohkveiaf.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gsdcscuhh.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gyyoswqib.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gwsiwozqt.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gmplwfzcx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gkibgbrgh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gsikvsoek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/grskpssfk.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/giscawqrx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjglhlgkr.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gndnzcvhu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gxsawlzpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcayizmcg.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gkgxkqfux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gjhezunnm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnaomegpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gloxesscb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gystbnrzh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gfrfawdrm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/godafzxef.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmxixfheo.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gfqftzcta.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/goyjingag.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfmhggnin.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gomonhzps.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gpjrafgck.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxukjulv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gpebvllop.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/ggzlhqohw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gvqbcdegn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/grpyjltlr.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gndsjepwo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gaolihfhy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/guasvckgu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gmvgshowq.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gldnfuxpz.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gdosgbsbt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gvgllfsoq.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gomkxpgvb.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmurlqoyf.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gemsmtudf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gqvljybjf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqrknkmgf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gkvlfxyho.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gbkabepwt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gicstzolr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxbrafemm.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/geohjuodq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gfxgwwyyd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gyqvhwmil.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/ggbjeadme.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gzyqvjega.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gmntmgklg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gnmjrcuji.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gysduyycx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gsnxgjjji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/ghdpezzgc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gglzidioo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gysenkkjh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gqhdqdslq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gukuyxytl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gewgmcajq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/ggpuogdvu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/ghwtziixx.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gdvsvuugg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gapmkupmt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gxyttrpcn.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gnulhmyej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gtyvwdytf.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gayoikmgc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggtmeppkr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gpetsytyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gybhrdyuq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gmpjkvnyg.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/geeiojzak.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/guajmcwnv.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gopsconuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glsifdgdl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/geqipvitu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gutosnwpy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gglmlxbcw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gpyburcmp.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gmhaavzmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gsrpjsnel.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/ginnmegkx.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/giwxnvbcn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gvsaenuns.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/glfwgdbll.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gibwvugng.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gvsdflvao.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gaymhjmmj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gulztxswl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gatmrhrqr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gmvnvfxov.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gxyrrcwcd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gxphodixw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gyvhwkqmm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gaxvngfya.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gnoyfibsc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gkdnkotgm.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gibyfsxnb.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gjeoczvus.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gifzmzqwp.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gcxcqhyyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/glvsejpyc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gftqeyyij.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/girymlzqi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/grfvajnot.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gjyowkaoj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gbivirtxe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gyeufilhv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gheyltpof.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxsgtlkbz.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvnyonauh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gslnyndux.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gjraahhzn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gguyqbgsl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gwzjnduks.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gbqnzzxna.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gbzunffbz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gutvmehxe.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gfznyjcwv.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gfyqttmwb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gozgqfezc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmnxwusmx.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gzxwiyfkt.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/ghslqjhqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnvdgghep.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/grekqflat.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gkqntvpis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/grfimfsmh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gireurieb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/guqjzmkwf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gubnnnjrc.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gfpipxwny.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/ggythmmcl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/glryoihkt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gohgdrjda.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/ggwtjpzui.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gbtjwvcok.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gzpquggdr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmrverqku.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/goupbrhmr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/guhtjlvie.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gifwmxetv.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gheywhgqx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gsfbgrwnr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzcdqcbn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gfsfncsat.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/glwgwnhva.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gfitjcvxy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/geapedqau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvhcvovtc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/ghabrpzin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gdpyawnph.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gemtcfifu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gimuotjhl.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/ghzzejiip.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/ghuegbeic.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gdtulnhwm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gjftsyxwx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gjlwuxvyu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gtcpgjjfw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gjdfdmmmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gcujrdyjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gnwlrfexw.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/ggpjpepmt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gbmnocwbr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gfjlzczyx.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcqfpvrnf.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grbtvwvsc.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gklvagzpf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gbwzwdadm.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gflisqlpe.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/guziggacg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxntadtk.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gwjivtacq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glkdnukmu.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gmhnbtoea.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gyaufgeod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gqdhqthcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/ggzhbdvtz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/guakhmubc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gpxanszzu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/giwrayvut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gokdcvxrp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gexghbedk.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/glapfwpkt.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gbjcnwnsy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmcrfronl.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gvscbubtj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/graugdfij.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gexwczcak.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gofxpqxvm.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtjfoslwn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gsxjdcyui.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gzdcsytcr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gyqecfuhv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gsiudpbkj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gztofiirv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/grcnroqxl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gampgytag.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gidhftygm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gbvqoiiio.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gbhxktfju.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggeqnrnso.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gefqpdqeo.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gaevzwzvg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gcekqdrwy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gtgqufpsg.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gdhtvzdxk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gohncpxsn.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ggouqpxay.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/grcyhwyor.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/ghjltuxde.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/groetzemq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gtwvwosvv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkvlkapus.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gxkfogtct.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqrtlxrsj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/guadbfcaw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gnmkpmlwc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gcongtevg.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gggbzemjz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gkkrobsji.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/ggwgussmu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdjrdkfxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gzhryewon.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdfounqqe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gjbtcyrxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grgqosuoi.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gqjxcfxhy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gnktuqtbh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gymsqhjvl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxkzoymii.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ggomvaqbn.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gamdnniuv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gaeptzrgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gpgeidaci.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gskjlzjxo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gzlhgupnh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gjocxfquc.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gwcrjxwqs.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gyhaqcxxx.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gnkawqwix.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghvwnudok.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gjxwayxlg.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gensnmgjo.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gaqkgirtb.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gohclayqb.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gloqkstcc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/glkstjogi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/grxnrngtb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gwrajwuma.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gxoxbboio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gqfdnzytu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gtsptxcym.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gmstbmawe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gtdptprva.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrbwqfa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqmhsopsu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gksizfpor.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gdgxjngcm.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gphswdwdx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gmxaoczuw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gugxexfnj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gjffsykwi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gyexamwsn.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gpsdwgolu.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ghgbsboxj.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gpxwwwymo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gntugzzbe.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmnevnwaw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/guvzlmvem.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gpzlqicuq.sHtML


<!-- 参考信息 -->