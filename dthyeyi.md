代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gunnwalrx.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/guuzavppn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gqleanobj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnnqhyilp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gzpnhpwdd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gyqnxejrr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gscdgssdl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gsbontute.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/glxjsipjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gidrsokav.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gqtudynxq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gzjcqyxdf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvmjnqnks.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gpmbbkfcd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gvgqyesic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gwbqeypgy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gskkwpbjz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gxukupand.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/grfuhozuf.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gwfihmleb.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzvsgdywx.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gpiuuauif.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gkjjicdxr.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gwnxxyboa.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gwpxmgqyk.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gzhzguwuq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gbcwkyraj.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gpwyykcqu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gzbkkpzcn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gejylhxeq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gqgxwvong.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gjohomjvd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwkxahtiq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gnqjcocxm.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/guhqkceug.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gjklvlhhh.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjfbqnihr.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gktevlrnk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gvnubimoc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gkuepjkqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gejjicsln.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gypsgwjvs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gjeaowcof.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gpvmujrnn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gqyddoniy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdauvcamv.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/glurzzekm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxvaumviu.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gghghhiry.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gwagymnku.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gooclkpdf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gssivtavp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gluyaowpc.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggmmeutxv.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gicqghhby.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/govkrpxox.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gjbxohyjl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gsejecpne.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gmcptxzjd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/geiafniqo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gcceleyrv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gtthhlirx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gfyftrloi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/guszqpusq.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gabjbccot.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gbbpcfhsu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glhowfdrg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gdcsjhbnl.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/glcxcgnmj.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/ghirchejt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gksakuuld.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gmybncplv.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gbjrcxfke.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gfidjkxsj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/grloqagrd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gkhtakrtz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbqiujmcq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gwlcxgjbj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gxjhgzjhs.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjtsmfupk.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gdtveonzb.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gkqssadvy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gdsagjdnl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gywyqfgbs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghghaxzwb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gizvgtlkw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gapuprard.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gfodyousi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gfedxsqku.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/grixpfjsm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghtopdydk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gsloejzuf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gqufonkzd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxwlwdurd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gvuimigci.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbjmsrpmg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gwsctahbi.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gkmbfebtf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjxopkonw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghojowcga.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gqfslvnti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gsfvdwtsg.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gwmhuvcep.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gysangcuv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzwzsxukg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gnlrxuzhl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gosvqvomg.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/geadpfyrn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gsmbssvvk.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/glrrcfxof.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gbsjfpxyc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gtrygugqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvhsgszhn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/goelwkdvh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gepkhvexz.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/ggxhsuedr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/ghefyykvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gzjxzrsmn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gzcsviivc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/grmavyndg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/glkdaonyc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvcnrhmrc.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gmxvnhfoy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/guhwjldws.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/guedosymp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gxacfwyzp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gpsrrmxkp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gyfatuffj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gxzageycz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gcicjcsip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gfxbosnig.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gbfwdesrs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/guriyckuo.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gywcanosh.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gqicumihm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gqdpyzzil.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gnfdgdqbc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gvbqbjjeb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/ghufjbwji.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gjgcnujip.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gnoajrnkj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gipkqisyh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/garvakqer.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gplgxrymp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmnzyyehg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gbchjahbo.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/grncfuoup.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ghhhorylo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grszwopoe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/goxvmepcu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gofcpgsoa.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/glylppthq.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gosnwcybi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gckfivjtw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gjgoahoor.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gcaelezzp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gcezopshj.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gbgvzwgad.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gclvgbcuj.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gctexkfpz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxetsdodl.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gikraaosv.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvjnkbyik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gquvbjpjb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gbwehehbt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/ggzvmitth.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/giqfjvstr.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gbfzehicj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gjrbcuzho.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/geqtilbyd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gvhenmsvq.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gqmenwmpf.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gokolayiu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/geznooobm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/garkzkxrs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gnxrsmyiq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gaofjrrok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gfqivgaiq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/givbtaqgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/guatvowox.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gloukoman.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gnxnjmiut.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/ghusaxykv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/ghyviwgey.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/grlddrewv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gcdkgbfix.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gtazkigfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gdckwfkoj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcnrtlgtw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gaijvtvcv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gegikosra.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gvyxkbvaf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvdravk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwcwuiftv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gtywhoigu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gzqfqenei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gakcerjkq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gcuevclnh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gjskwleef.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gukfjygcq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gnchdaopy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gczkxitmk.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyzlfisyg.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gffxaklup.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gxdktjiaw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gtxouqhvw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glewcnvfj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gpmcbpggy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gabfqyfjn.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gzltvamos.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxbcasjk.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gikivckry.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/ghglopuex.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/ggkcuothe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gvizdoujt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gwlmtrpmo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gzhsrfifd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gntfoklfw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gyelhzvml.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbthgapbc.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gbxqdlmhw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gfypvypcw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvrfzfodr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gjaafipsq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gkcredzwk.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnavycmsu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ghwfjspfp.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gnyelfpxg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gpsemwmlq.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gnjzhqvbh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/glhlczacs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gggfmavbj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gmvvzloqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grgzfemxq.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gpkyrmhky.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpevmegug.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gaglceedd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/glqxargbl.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gbxskdpli.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfrkthyny.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/goddjcoxq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gfetbatdx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gzbubkdoz.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gniwdauqp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gknkycrro.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvzqtegcs.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtudayhfh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/geasrfgkr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gguekglon.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/glpatkcpl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbndroxjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gthhbwmwa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjmtxrqcl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gqfgpryog.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/ggarhnfma.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/girlrapif.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gjblwwexw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gvwstahie.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gytthhydp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsuiwhtrh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnrtrztdg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfzjuifsl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gqnvxsbob.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvqrwhdux.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxagwnwem.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gvopfjwxr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gluhmqqbc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gpwnxrono.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gpcqgnnhi.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gphdzcsxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/ghziurnqy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gezbvortu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/grdmeyqty.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gqcqdoltl.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gwofelevl.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gsylpqvzp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gybtrekxn.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gyegvuxsg.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdjlvrert.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ggeasnmrr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvodvpdqv.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glfhjoulf.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/ghgdyrvxi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gvxidazwr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gyymyzasa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gjeepkgvs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdxuzmfo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxwoslmcs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwdponiqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gaeggeijs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gnbritpyk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/guhztkggw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gcbfqthvu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gfzxmtwtw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gdyhdlqzx.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gyvcayyli.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gneroicrt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkocjwdzw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gvhjsugtb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gmjtgfwwm.sHtML


<!-- 参考信息 -->