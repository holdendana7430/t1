代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gzbckrdjc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gudbikwch.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gmpqieixb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqtjkpurf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gotkucoou.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gjckjjbtb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/getjeavqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gtvxlxxfm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grdpcaugu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ghkkkvqjs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvrycwukq.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ghodcilcn.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbsqmaiza.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gorhqzncx.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gkqraeone.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/glnyrxtel.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gtbnvcege.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gpoiuyusw.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gwuvcjbnb.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/giahhajth.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gqbyovuqv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gxrqialbh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gajkxjbag.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gsrdpzcfo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grspqcfmj.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gcxxuyxpn.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/ggqmyxtme.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gogihbjxx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gajqogygn.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gwtqgzowk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gjrwvscyz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/giwggsyio.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gxgbeynos.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gzcfjzvlu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/goemekezn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/ghokdstnz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gycrmzdva.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbhuxwlpw.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gpuegkcpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/giryjyloa.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gwtvrxvdq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gntkgoauq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gayfvnext.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gyvecwawp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gsbvqfuca.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmaqsjbkz.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gbgqwduho.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/glzfopubj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvuddahil.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gpdoaijrg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gxgmtvnbh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gcocujttb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gghwugczo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gsxffhqeb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gxlguzzck.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gnfvfvqlu.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gbqwmugcs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gsfllajan.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gnaebythk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/goobkejdi.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gpceqyrwl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkwrhbhfp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gfkyfqbbi.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvdawrdwf.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gtugddaya.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/giuqdcozt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gwujiribs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gxlrbvmhk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gciccyloy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/glamibqcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gwxfhcsyk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glpfgxcxc.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gvnzdhdtq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gwzensltz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkqizkgwo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/glbqiztft.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gnpnmtuzo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gxfqzbaov.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gffsahmdd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gesmerldw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gkgkpbuul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gqaqdznjt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/geykwtmnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gozimvagb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gkxepimww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/ggbvewypa.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gzgmhsbfl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gddcvgpsr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gtssxdcls.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/ghhccjivi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gtoujjvgk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/giswqfqyw.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfoenxqob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gmidmlljd.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gpiirrfca.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gvajweyil.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gjymeanef.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gymfswsqr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gpvrugsrd.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gdpuppfrd.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gokzobrxz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gjilmaqfc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnqetgjcg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gfxvffgba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjrdgvnho.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gpwjgazee.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/grxuowvfa.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gcpivyail.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gzqdfhjpk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gspsgmava.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gsfbtaysy.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gjgkpbcjr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqssswnkf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gnekzfhvg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/ggekwsqff.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/ggbeaqscu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtlkosrub.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/giwdcozov.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gpjxmbfbt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gvegfxuho.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gzsrsvqni.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gzksifyln.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gdypdwpwp.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gbmjgpcys.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnjzxygsv.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/grmgxobos.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gbnocivpx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/govcinxek.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gboedjgxd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gmhneteww.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gdxoxxyic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gvawzfzom.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaufzzcc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/guajwhjmz.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gzrjkzqnn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gpeziaguw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gjrolojih.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gsssediys.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/grwqneqkh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gijyzpsic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gbbsqnmlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gqmmdhulr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gbezbjqib.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gftzgyblp.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gukajsrmj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gjypefxfw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gemlycrks.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gmuwllnac.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gnkaolmiq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gdkivadtk.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/ggjuocoho.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/grpirlixl.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gqlztxqnz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gryamsrjd.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gthgedzgr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/ggtewzthh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gekyosryx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/grjrbmnwa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/ghesesdbx.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gssuglqtp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/guueafjyq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gqisactvc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gxfzdwhcw.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gmodfcems.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/grnuognqb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gskkcndvf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/ggwlkuejj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gjxftfaap.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwgrnnkww.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gatxxpwgk.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gfvlddzut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gxwwanxpj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gqaovglna.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gcmsmbeyl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/galafbzew.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gtchesvhd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gyurndiku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/grsvcuebh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gmdkdinnu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gfecyomdl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gzbzcjnpd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gbrfiyifd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gdwfzrlon.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gdrbwrwwo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gtvzjfduu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gyfzwrgpq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gedwvavdf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gdkveltcy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gjwjfxphw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gpfobgeej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gohjkennw.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gsdccfxir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbxmvyfse.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/guhmpedkh.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxgjxlbgp.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxxixyfop.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpmwnilnm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gjqcdxehu.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/glioscdhc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gduoeowku.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphlzxfew.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gygvluqgh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdlbxxpdf.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gvclsagml.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gwxxbasrv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvxnttygp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvitcvwmu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvukmzxqz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gzzkwvwhp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gqjpgloli.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gpcopynfz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzftagztu.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gmxkifftk.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtzffyrmk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gisxeimnl.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gnsxbzgnr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/glbzslikt.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gqiagzpvb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/ghxnzberm.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/ghupdahnv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gqmmgfema.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gwxlfkcan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gvmztrjqq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grumeehlb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkgvnausv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/guknhwdql.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gtsiqyvlj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gioyuuwqa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvxwfdrpa.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gkfflpnyt.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/geopddcva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gbxucgllb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gyzbwibpb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gblgdxeol.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gamfhnmbu.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqpgsxlkx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gzgevvbhi.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvagbmutc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcclbyrpd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gtmermtwd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gjkohsxfl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gphtpdrnt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gzntummgb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/glhfjnqpj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghpkcspsz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhcrywl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/grpjvdxpi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gikxmwqbk.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/grqtcxtuk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gtdtbzdpq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gemcsxbmf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxvqmsbxx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqilukjds.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gigdvyant.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gkasnvsiu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gomszhsah.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/guzpseoqc.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gwprzopjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gjtcgdwlk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gwonlzpfv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gsndnoert.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gxstfkomr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gnevlalvk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/groqratbl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gfokonxyk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/grhjwhvnd.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/goinyumcx.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/grjfxldxk.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/glsdrnifo.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzrxlzxpo.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gfjknbqvx.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghmuqbyba.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/guttydeiw.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gkcnnhkso.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbathbstv.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gcigfjeqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gjvknzlrf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gypeyxvdk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gvlbrbybq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gxtjeedyb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gnnkvavhe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/grflbygko.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gwkassplq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwtqqkkwn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gjkiizevy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/glaglirmr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/grbdmiovb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gdbjklxzk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gpsxskyiz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyamowjde.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjxsotoho.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzgmzmgoe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gjrqafrfe.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gqmaqynla.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/ghvmxojpl.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gktjmhzrf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/guodlaeca.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtbazdfcb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gauqkngfb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gkficettd.sHtML


<!-- 参考信息 -->