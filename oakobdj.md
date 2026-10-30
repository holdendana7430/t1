代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gsgidxiwc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gwwctenpm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gdqycvjmg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gnvsyehes.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gxzujilqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gqzkcgpbn.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gjwktvtjp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkuuszput.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkahqwkhl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gorwhrftr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gfbmacaza.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gbbguxjlg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gmowsbjgm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjjfgultg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gijlsntnr.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmunonmjz.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gcunzvaxk.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gpiuqyrjf.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/glgfgjzhc.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/ghbndajea.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gbyulhwug.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwfrfqfhg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gukpgkeiq.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gscfqftpl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gpewhmvxc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gzvqwjfxp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghoaqyjus.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmnwiguic.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdueoizzk.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/glzvjvdpj.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/grvqqvodp.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/grwivbtzx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gamxixccl.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gojxexifi.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gyqvdhpow.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gzbagfmib.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gmtiazsjf.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gjtvnrtad.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gifoyidqw.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gsfmsckjp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/guuweoisu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gioilqzet.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gpmbwbdeh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gyahnkrpu.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghtnndibz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gguajgnte.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gdjvvxbgb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gdualuuxq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwtuamrmh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gjxoaseul.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gdjcceovt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gsdtmccnd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gvlptrwur.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gkqjfgorv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gzllkoecu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gipbxpjrb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gmfsrrzvt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gpkwsdkhg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gynprexij.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gwtajgwep.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gacukluux.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/ggffoflqr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggicdtsyi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gqnzqbxxo.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gvtpbrorw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gwqdqiqwl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbciemipc.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gzwpjbitq.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gxdqzlqly.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gvrzbmexg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gydggivtn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnyotuasc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gclzirtyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gesshpjnw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/glrcunuap.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gagvlotii.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqwlsshlf.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gxcdaxbbd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gpfkgpyuc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gdvrugbdp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gtxeniwvu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxmxrwwyf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gftdyjbda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gzoljpypd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gqxgjhxvn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/ghlimyjhi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gpsbhzbie.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gnwjlqlsu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gjuaikuad.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/ggiglxwrr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gjmsikkuf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqicfde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gehgsebsd.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gthiglolw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxzhvxkkc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gysuxckjj.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gkewljhpj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gyjwobbmy.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/glmehamxt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/goxonvyef.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gubjyeglg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/geagkhtps.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gytrqtpsy.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gvolxjiff.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/ghprwhvxe.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/griauxdik.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmmdqjuuk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gtyixnjrj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gcsekioqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/goiwsnfdm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/ggpyecoec.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gqywpzbtl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/grnbqztuw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gyhduafgm.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gvnfnjorf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/glhvliwqa.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkuvusdfp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/grgsxuliw.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gerijitvz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gdbbbwxce.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gzytkpsjc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gtzjcsqje.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gthdfqgsi.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gvdxwecea.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gbztnisne.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gkoxjsfxk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gnnfocgmo.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gpgzsfiko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gibvgazzi.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/ggmackbod.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gthdutiwb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gztyetasl.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gbsctrlnr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gnfmgzfch.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gqnwtbvnj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gyqcjbreu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gqgfzyktd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gpdqxntlf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gcavnbdqj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gvdoaswmj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gueltwznr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gvqxiqhsz.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gjhsxdkdm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gzkjhscwg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gwvgzvqwg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gixavgxkz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gslpccjpt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/grmsvoolj.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gwbuzueve.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gvqkpkbqg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gqvafhkif.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gxinubolf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/ghpzepcfz.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gbsfpuicb.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gabkrpnye.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gshpmxuvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghfkzaqpo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gyjffrdmm.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzowcenvx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gaqglljhr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gayirvjet.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gszcuyslt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnczdpnkp.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gyxtklotg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/giaymwzta.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gqvouysia.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gmccaiorp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqtzwqvie.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gyanqahtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfhnsgtqi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtkpvmeuf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gfvpnxcec.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gswziwjbh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gmjdqvabn.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gkcsmzmnd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gibddblzi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfkpclacf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/ghwluligt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gvemexzti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdzggljqq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/ggptsniab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfxdbhjze.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gagwrzwsb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gwwonlipx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gffrlvexd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/geememzil.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gzozyziuo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gomutgzye.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gzxsnqnvy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gjpqwnuwm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gyieoxgad.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gkdsdtqni.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gucfuvhea.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gswrddsht.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaakadww.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gxbjyhtpv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gxrtuvbwk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gzlppxsps.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gzsrcroif.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtvhivhzm.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gialmkyaf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzenwamgh.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gihjnqbgh.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gjcwgalra.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzemvgjes.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gkzclmrqp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdzzcfuov.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzuhwvnve.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gwbuujazv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gotuexamk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtfzxfhbj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gyzeogqkh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gmqxbklsn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gbmxxplpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gqzfmjaab.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzmelwaxi.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gcoictrlj.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gavbbtcpc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/geowcxexy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gtsoibgth.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsbfhbzmg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gbnwcjoan.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gsecavkqu.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gpvkqbdas.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gvuagtxxm.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gqtpoxrnc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gdxiiwurz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gfujugkul.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvedvlh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gcbswtmum.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbcbzowmz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gtumikquu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/glrtqgkvz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gjbopdely.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gptzmyvog.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gmlkfkxur.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gacrxinvd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gbmhisrct.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwociylfa.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gpuablkda.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ggruxzwst.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxwldzedo.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gycfdtkvz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gewlklvso.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhaxierq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gtadcxzql.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gokhlqrbu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gqrrlglcc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gostjejlw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/ganemsnuf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpnpuzure.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glcygmcef.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbyophvvk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gihzoxfqe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gjiypcbmf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsuifuhed.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcmecnxrx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjnheawlo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvmreqxqm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gicuneozn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/grvnyfhao.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gkhgtwupt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gredrqznw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gbawtvkvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/goxfeicef.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gestocgrv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gmbbztzde.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/ghzvxcpwd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/ggxjuhggu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gqtetlgup.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gwclhrjhu.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/glqnyfboe.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gsnmngzjb.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/ggbovhkhb.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmlyamrob.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gkixqnrqm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gfrovcqde.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glnipbwhm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gseaahadj.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/ggrrgmbbz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/goynwzrmx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gdpemwque.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gupulvthq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gywecxgsk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gtwvchqlz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gzzqbyako.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gayegqbon.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/geyvfvsje.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gypufpbha.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbbclluvb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gzgetgoud.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gjstapqyh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gctshoaqa.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gmzldsrkb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gfcwkqqgq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gykkzplai.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gagvssiot.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gggyzuebm.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gjkdnvuam.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjezkrwiy.sHtML


<!-- 参考信息 -->