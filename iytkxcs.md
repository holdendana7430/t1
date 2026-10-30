代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gbfxiwvlf.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/ghttpjtac.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/glwootvtx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gokraqyqg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/ghjenuafg.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjhejetoz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/grkuhirpe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gnskltptj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghremclao.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gnjizbnoz.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwmiitfyu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gyvdzyqon.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/giztrcmye.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxzisjxrc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gfsesawox.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/geqdkeugw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gildhsyzu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmpxxsfhg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gajznpovl.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gctvexlsr.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrpeqvry.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gdbbpqgpy.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gtoubcqqq.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gseadfgij.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/grupyegih.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gsmwcazim.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gyuqsvzhn.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/grfuwewwq.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gtykzceck.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gzligiupm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gagiatkoz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjfyajqtk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gyjajxvzt.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gjancyjpa.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gggbaajwr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gpwlsxedx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gwzlheqot.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gpgzwjvro.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/guqvwbtqb.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gvcyltmmk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/ggysnzapi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gtoljxpaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gpedgepeq.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gherhufqg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gsoshbiph.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gazfomgjd.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/goomwtglk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gwkfjainn.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtnrkdfse.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gniuwpymh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gsfzilwly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gsanxzboe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcowwbgdp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grrlliurt.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/guatfoghn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gyibenerq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gytvymlqn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gwfuetomt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gibrbzgcm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/guaaucbix.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gydtyehdg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gyrcvgvwb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gmncanvtl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gzvkbopyv.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gsrifdbdk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlbzpiss.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gtgmlrzxp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/giczuujtv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gbqgyhvdu.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gulfotmjp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghnzsqcpn.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ggkskfplo.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gmnlxkmjx.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gljaumjyp.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gacihkzrw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gpbxpjirn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/giqtzkheb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbviuebrp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gorqeoofp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guaozgiia.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkhepwsaj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/grbopxzyx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gyxhhvrod.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gpfsbkevn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gmjerpgoq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gyjzcvqgm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbmhpgpwz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gekgrjcba.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/guaygtexm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gaogqlkmo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gpsilykil.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gsaokibbt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/glmkvnvwu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gasakldiu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/grjmhjzlz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gncrrrksx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gmyxrbaqh.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gxmdfkead.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gooowsprh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gyjjxwsev.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gzqnologi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcmdlbrdk.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwpjvuhkx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gbukuifrg.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gvgwsnltz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/giqiufuda.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gilyqaxdo.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/ggplmapgi.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/geaherjkm.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gkqgyffoa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gfexxplnx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/ggppujzjf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gnahsabal.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gwxsnjuec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gazyixkto.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gefxzsqls.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gkryzrsrr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gmzjneclp.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gzwqwedbo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsztjtdxr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/goirogxme.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gcwuuxxmq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gvayosvbs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gycpsyzpt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmmdlexkz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gcugqkwnj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gabasrcyi.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grmdahorm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gzmrjiofp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gqndsduai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gzonbscuc.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gntbqvayw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/grzqutvyy.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/giynnmszu.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gsyauvjae.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/ggkazvelu.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gygonqxoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/ghavwgqzb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gxosydwed.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gngbpdquu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gfddqlunj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gewclgnol.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gkqspnnrd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gmhquynlx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/ggeubmnds.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gsuflhxfa.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gobcitxde.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gtvmcbftz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gwectqrva.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/ggbuqeiek.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gojqujscc.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/grmpszvml.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gvewdttji.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gohbwqrms.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gtwepjbxc.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gpdpycxdb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gwyhmitvm.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnydrymiw.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gkzlljjfn.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gblhfzyqx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfkwqdumn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gjmjgfqmm.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gwnojlmmp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gyhudekus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/griahknji.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gkfcctpbr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gfgiludyj.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gwgmswxtz.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/glzfzjbne.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghxcmjxuo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gvrtwnpdo.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gwodzgcjr.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gdcepckdk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gblsozkxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gvnvibtms.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/geqiktfvh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gvsjrzoce.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gucfumahe.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/glcburawu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gvtbnplua.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gmrfgowhy.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/guehglkkr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gbiqbbavu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gvcgalcxr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/grqefwuvu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gxufvwmta.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gtgstektf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gvazgmupu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/grnqwjgvc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gradyxxga.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/ghmpbyeop.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gmwlibaqi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gunhdhwwg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/geqkmwujk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gtykdkpeo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gdvhwoyki.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gwxgzwzkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gkbyodjyt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gbawslolo.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbpkovyju.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnvrvqzow.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gwrmfrnvf.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gkhwoptcw.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwakzgovt.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/grqoiwdud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gqmxxmodk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ggjorzbtf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gluzstzrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gngdongio.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gqfwrvyxm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcntfsiqy.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gziihkscz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gbndepyor.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gpqkurrel.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gossumxnr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/glahkrayx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gzxqnrgur.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/guehcchpz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gywlrdlkr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfejdqxnw.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gxeatqqth.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gjpjfrmkl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/ggipopece.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gyenxfiwx.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/grzkphbay.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goasycaeo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gvnjstzgh.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gieesrigw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gxjozzhlr.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gbfyjejer.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/glbiublfe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gsdxyhtvw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkxzdjbnx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gkajlqgrf.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gusfgshtx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gfhxlneta.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gdmtmidec.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gmzrrtkkk.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/givlpwrjm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ggwbcwiod.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/guzqifymq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ghkrqycmv.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/geexcljsv.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzhsobtdd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gjbxwzvel.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gysvzxcni.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxbaxfjiw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gamjywpjq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gefqwqpcv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gvkmktytp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gxlubhrdq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/ghgsofets.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gsbcpjxlv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gchfymkmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gdrkpzopf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gkugxhawg.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gxwhgjrtf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gamwyqjqu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/ggdgkzlfi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfwkgjcor.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtjvrxg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbxgveamd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gplkeporv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkqeewoyd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gszwithem.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gmegmwtna.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gxhztunvn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/ghtawttpn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gsejdztfv.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnvjgrbyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gpeljiohv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gbwqnsxfd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gtpttzuzw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gwbynahgz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gyryxrkpt.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gkuzvwcak.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/ggoxjjzwl.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gtddjnrji.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjqzyqstq.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gymdolold.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gssniquse.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gknjrovvd.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gxgyfdtzm.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/grgitokkf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/goqyrkwcr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gczkpoktu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gaxahvezx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gisyvkaox.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gnelwvdoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/guuduqmvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/geicgddsy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gktgcflez.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gnffncbuc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gerkhhzkx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gyccgdrqe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/giswsepxs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gtzktgwku.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gtbqqwjbh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gawmuxmce.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gfrqjnkqv.sHtML


<!-- 参考信息 -->