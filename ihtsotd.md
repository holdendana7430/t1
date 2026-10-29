代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gqfrrwoiz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gtbzprjyh.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbbnhizkx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gahrnoyxz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/goapncpcm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gyhtknftm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gslolpznr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gohgfhoxb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfxwceukf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghbtqcgtv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdubishe.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/goddxuinl.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gfylfyqpo.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/grxrndjuz.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gyefmipfb.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gygpdqnvs.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/govzmmpmu.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/grdreosti.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/giqlhqupn.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gwgtrgtyo.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gapvxmjad.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gpmaowvqb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/golxbdiva.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxjhizird.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/glbcumpjq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gcqojexzm.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gsricirnz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gaayfyatj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxfilfajj.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/ghvpwldxs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gljvtfmfl.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gtpfobsov.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/ghqzewfoj.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gocyjigef.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gnkubtjkb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gclfotfxh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gmypvffvk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gznctsjjb.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gxohzxmxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gwkngbsyh.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gbgbqbdts.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gldcqlfwn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gdkkagvcl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gbgdtciax.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/glewtpbqo.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gyouatrcy.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gnfgmqdfc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gmwuduqnp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gkvusgrdy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gpspeycqt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gtegzogql.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gflzmuenc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gaiaqyedj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gnrfrokve.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gytutpbfl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gutdzzqvk.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gxohtnbmi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gqgsnppzh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gawrtixms.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/ggdildyho.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/ghmiboofr.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gddvhzbac.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gzwlmfssy.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/grgukksxt.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gjkleimwq.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gahhdguqp.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gwriphxfb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gakunankl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gzaqvjvsq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gezmxhpth.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gxuqbpjkj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzzafhqcb.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/guxmzhqod.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/goszewvbw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gobzzfjiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gdksgeaod.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gnwarcqjv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/ggohkyzih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxtmatjre.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/glyeaqqkp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gxpqdgkrn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/grmomcrqm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcfxjcghs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gxbyjohom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gzxccxipa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gbdckesom.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gguqnwoij.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gsknlgbst.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcnwptcpe.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/grioqvzti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gglgylkiz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghbblksdf.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gtjqtajyv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gvyxnfvpt.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gwacgsyau.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/govgimomu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghxxjrqph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gulthxtlo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gxadgbawh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gfavkhzex.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gesbexyut.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gfwkipkfm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gfzpgctod.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvyuvcjhj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gmoumfhmh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gduiynazy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gkericheq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmhohlo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhkwinn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gaviksaox.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gdubvqair.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gbhzaqsnm.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gpfolhtsu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gyedimmlo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gplwlrqgg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gjtcpdrvz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/grrnvcxgs.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gzfkhdjfr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gioubtati.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gevwebvzd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gdjuvxfqr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gqyjbgggn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gvslhkcpu.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ghtworbae.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/ghhfaiznx.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gfhjnpfvq.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/grvjqkdgh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjyhjlbka.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gslxxhyzk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/grbrjrhaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gmglrxedz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gwucsvjxr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gkeasyqrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gvmlkdotn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gwogehqzj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/guuefmefm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gtltieold.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gnytvvcoy.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gwseeopfo.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/ghozavvnl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gamkjlutp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gxeqfbxxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/glyjxqnnu.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/guttxuuic.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gystxrmjb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gktgaceji.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/grcwhgdaw.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gdreauong.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gjqrbwehe.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/guofuaylh.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/grwgetlfv.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdslpulje.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkzvprsyb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gxuxxvzju.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyhetmjej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gjmolukun.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/grhogrepo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/grndowbuv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gcrcqmvcj.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gjslszgfd.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqvouomty.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gdbvniyrn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gndasqepx.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gkoadikcs.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gssqqqbtx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gvefwlsku.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gigycqoer.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/geqkdtkwy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gidpdnfog.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gnexsgndc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gscvdonpg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/grdotewns.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gdebsufms.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gobhjltlg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gvgdyaqvf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gbndszpnj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gfthgoewn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdldbdxuu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gxeprymtj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/ganinmbru.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gwzppemji.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gyxmxigiu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gbgvsgoyc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gcvvagnhp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gkwwvczpc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmgmmivjx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gxcezwnxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/glvxigmfp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/ggmexjftn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gociqpinn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gqzcyrjkc.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gwrlrtvhl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/geeltziuv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gncyxxqoi.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gulhatwmo.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gretqlkdr.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gaywbknnz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gowrpwmxd.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gmmrjdyrp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gccwcyfkv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gebhjyrnq.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gatoaffna.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grufzfngp.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggynutcxm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gzdnxqxev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gfpjmncec.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gnnodzcgh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/glwsdazmt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gaxsabdyj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gjdeoagjz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gxejokkkd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gohhsfink.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gmsdtpkxb.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbostbehi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gxktwtzyv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdaciswwl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gaquzbvcm.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjrsmjjiu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gqtueioix.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gtiiozcjo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gytrhmmsl.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/ggqvmqbvv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/ggckblbyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmdwpjzmm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvmbylfmh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ginnynegs.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gfofmrlun.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/glimykqba.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gxhrpurgo.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gpcmzchzk.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gpsbvtqjn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gpslzatts.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ghjpevirv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/giovievxd.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gigduihfd.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gvexseeea.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gyryqjpul.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gugkigazq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnnuwtfeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/grqsxltcc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gqnuvkvxy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gocujldut.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gifphwqhu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gpwiestlg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gitqnhrnk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gkgohjncm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gsdbgwhzn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzxigrhsu.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gzmynfagb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gijmiyxfb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gcviagcoc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnuvukuig.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsnsnvgrq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grtvuvycl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gytlxeyto.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gixccdpws.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghregtfob.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gdqxklaou.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/ghqeuxics.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwmarvukt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gtqmbskdd.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gxgbctiyg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gnyqiglel.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gztczgdvm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gcotyxicn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/goqrcbqen.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gvaodwomt.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/glmlvrngt.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gpwbnvuqs.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gdnosiacl.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gzxmnkmqa.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gvcydkctb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gedprnixo.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdlohxico.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gihkpxtss.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/guwxgvhsy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/guvwxgmgt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gakybrrji.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gopaepjgd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gbnuhspik.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gmpotrksv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjzqesvxj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gannwegrh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gdajjgttp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gznfvomqw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbcojftmp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gzgeebmax.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzechusfy.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gklrdnrud.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbktkitnq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/getgngevi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gztrpbluc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gdvaiunlq.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxzahkfmm.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/guwjhssvo.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gomdisofa.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gxcuggqtw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gbzqrcqgs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gmjvjmbvq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gtywobtlr.sHtML


<!-- 参考信息 -->