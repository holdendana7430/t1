代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gmvomsvyj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gthxwospe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gaytnxvmt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gbarjodza.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gvwwidyqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gyrqymijj.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/goxttubxn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkecuyckq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkyaoxajo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ggfdtjkdy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gsvzmgjld.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gfnvsfdkh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdpsqmiol.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzkqeslsr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsthnwpgx.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gkmxvahsu.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/glziyniog.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gedmedqwi.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gsgowjuic.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxteumsfj.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gwuqindfi.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggfrigpgw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gmxkqfdgb.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gcesmlguy.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnaazxumz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gxhshsmav.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gyxssiymo.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gywtbawjl.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gtdxgmhhv.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtwtcsivr.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gfvbkrhlh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gmpyuvmgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gvvsgyvae.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/ghxvrvyhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gizxkemvx.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gcimnzzmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gaelbinsy.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gfksmitnh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ggexftwen.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/grzxeombe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gncbsttug.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjkywjtec.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/grjlvdlce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtjmblqym.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ghabjiett.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gwwbpycow.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gdzfumzad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gsonudibs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gixhyngkd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gfdminczu.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gluaegekj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gjbbbpnwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gxubnevfq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/glntxeqog.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/goivchmox.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grbjgkiak.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gxrnefyhg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gtzjwxcah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gqcuvcrvt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gdaykfivh.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gxlyxlols.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gxbzlmimw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gttgbqehr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/glxgrtnmg.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/glurtorpd.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gufiijdcu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gbbuqdbuu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gezjwblnr.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gwwfukrap.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gpdmopcir.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gruvxkebj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjbgmuejb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/grkjmlvlo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gtayrimrq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/ggkcoydrt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghtzgswcn.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gqamrezuj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gitvpqorz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gnjflckyj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfxmlrcoj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gvozmavou.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwlzfcelp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/guxcexpea.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gxvevvova.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/guhtyaxma.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gfhrmsazu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfoatsqhy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/ggnnjefwu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gmtluodfh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gzlxezwso.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvhbbzmgm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqxahqabp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gnjkpwufe.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gtefcwrmb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/ghiwaqdvg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gokuaotem.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gvjsvpwec.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gehbkzumb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gooqzqcpo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gbintikph.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwfcwhrkd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gtwkwdmpg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/glvmwrepc.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gjsxxnszt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/giwteinqb.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghdhbzmae.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpjcyhgev.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gtuebbklr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gvckplnxk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gokguzihx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gsdichiqt.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/glnggshzv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gsdqajluf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gufgndegv.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gdgmpzubg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbixuvims.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gsylylmsf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gjrxefspf.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gbsatgdeh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/glqbuytnn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gxxgodjmr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/grrgrdgpi.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gmyxlfnyg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gyjxgpsvw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gpvcxkywb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gkculdkcf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gtieyfatb.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gfcuilbbg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gioesftiw.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gtdhwasvy.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gugokqvbo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gulbzdnkv.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/glphuyvtg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gkjhvabyn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gsyhihjma.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gdokheunn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/giwjxujxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/govhmvlqs.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gnnpcyxdx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gvxdytpqb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gdbklydur.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gfrhnzdfg.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gzpkosgee.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gbvmvcytl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gbyqmnjzs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gfrnuzrtj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gyosysraj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/grgmirwwo.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/grwcwgkkt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gximqbvak.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gfkuijnhe.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gioorwzrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/giekbkmwj.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gimxkhosf.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gomknghgv.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvnzjhlpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcyusxqsm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggxhixtxa.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gabffjuvh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gcliqneec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/givapuwns.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gznrmitlz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggaqwsllg.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gorekyoik.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gwpenppel.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/grsfqzsha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gvnhakpvk.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gevhbmmcw.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gfxnyseul.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gjyvzsgdv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/geyyjudef.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glkxympya.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gmctapnfe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gvytklppl.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gezoroxvj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gtlwkzijh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gfvrgajfc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gpreaxqoj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gowuzcqab.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gnkfflhzv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gfijainad.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjausekld.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gmlkqxlkh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gzhyfjeye.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gqzwgxdcu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gksbainne.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gezsjrzmc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gdehalxnc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/grzadgyog.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/goeawfsdv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gwefkbaye.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gssllccoa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gzqaawgbr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gffbxjhpn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gzsyrsbzv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggmoxkwxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gamipqegy.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gehpnsnqb.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/goxwulqht.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gogkmfpjm.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gvibwvjcp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gtegpastj.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gbfxqrvpf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gewsbcemb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotdrumqf.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/geeexjdne.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwepzrhym.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gritrmjrx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gpggflilc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gasdzxazd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gpmceerwu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gblrtfjrv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gyrsdejhy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/ggfpclusy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gandgfiuj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkyeoskot.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gapxdsqka.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbvgkydvp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwogcpfjt.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gwdiwaihv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gzfhxxwti.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyjmkbrqq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gmzvbizbf.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbcmpgyav.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gzbdzjwmn.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfghsgrhw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gksyjluqv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmazedhxh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/goopxqrfc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gstcekrlc.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gowvdeapn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/ghxzuzefv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gvlsrvhbj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/glvxswgnh.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gagypuayu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfgaybztj.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqzdegx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gkeqndlpg.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gdubxehtj.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gphxlawqu.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gquubaohl.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gmbejwbay.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gixjiveei.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gzsvzewjv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gcqehmbkl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gootcxlcd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggujraycj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gxftrdjfo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdiborfer.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gfarnvyfr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gorrzibix.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gzvzmzoyz.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/givufgdfs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gitogmiki.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gekiyehjc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gtxtgepok.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gchkpbzbw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggbuvbqwg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gygymbavq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvqyiifxq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnnodelss.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gyfetqogb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gyupqqykl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrgzhnx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/guihneftp.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gupzhywxr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gxbffvctl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfigfbiw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/ggggbhjps.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gdfspjhkj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gxqtryyuf.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gzjlgrevb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gjievfylk.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grgpkszun.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvqbwpgpy.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gyhtskcog.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gvwkcihct.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gispapiiz.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gvfayygoj.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gdvwnvycy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gktxtxqti.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghgicsaiq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/goviwcsrz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gjndvldbm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gbaeijrte.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/giuvobaya.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gshdbeope.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gfkukrzge.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/guhlrnlpc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gqfoklixn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gdfovvtwf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gzgzpniif.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gmdrkemxd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxxrwzpct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gvjbtbxhz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gaveksiuz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gfincpvrh.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gmbknlqac.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gklduyubi.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/goihugiiu.sHtML


<!-- 参考信息 -->