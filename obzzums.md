代发 wailian999

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gwzctlwuq.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gcaqgypwj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gcpaxksau.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gldkbgcfh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gfgiirrtq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gjxsahpov.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/guowfjvwn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gezjmmqjm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gvjjrfkla.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/grziifmfb.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/ggdrcxtdn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gtfolmyvg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghxgkymun.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvuoijvwx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gpswrttml.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gizmrahpp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqosrgnmi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkidfoigy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfnkffsdq.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gemyesgym.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gtxtdtplz.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gloshkhuo.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gqrccxypi.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gkqflhqxb.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gbfszjztb.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxhvuokag.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gcbvyxsin.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gtxgwhkqn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gbfocuvve.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gzmvjknbm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gcsjgwbrv.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gldsdbjdu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gunbqycgh.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gysmqveld.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gzvaowajs.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gestfozia.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvsskufxb.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gyzmecleb.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/grmgdldnl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gdvzoncbo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/ggiduarcl.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gpiojfmhi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gtbswfrfu.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gcrclnvpz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gzuxdeceo.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/ghhajwxgy.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/glevnyvbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gygzegklf.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcxdlrgcc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gqjgpzpvp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/genwrzkwz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gvdnlshom.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gluhytodt.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gtmghgbcc.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/ggnlgceyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gsmbkwzlz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gjivyuzvj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gmcucrtbl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grbcmibkm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gdztrkmsh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gnxdcazjg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/grormawxi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gzhoqasbo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gwvcmfyag.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gdfumnzgh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gkahkokvw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/ggihzwewe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gboxijewl.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gwqtouayh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gapwpebea.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gmqzcgniw.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/glzfpumyr.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gjeirbxly.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/ggymwpapc.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/giypryxdv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqhculzsh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gawgqutqh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbsisvshh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gnztojluq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gihbofdna.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gcirvkrve.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gdrvvlbjb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/ggufssxtm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gubxrprco.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/guplryiif.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzhsxigix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gslkalunz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnounggvi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/grheaovuf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gtuqcqfym.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjomrhnyz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gezibydrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gpmvyyuli.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwibujwic.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gwwvkrvet.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gyosikmpw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gfigdiljh.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gigsagltu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gereozpea.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjdjuafup.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gaganvzxn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ghjnxwrfp.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gtxcduzgn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnimybolt.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gaocydmhk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gwbzifysm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/goczpfeuw.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gglgiynsb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gdpibegpn.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/grtaszqqu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gaxshiurx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtwbuyhkr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcyaozwrs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ghmuvanwx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/grufyipot.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gktbvphyg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gwcodsjdh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gprxgxuan.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggadutmoh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtexgltps.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdswqptkg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/grhemcqkd.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gymqnjika.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gmpacbjly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gpqxsxmlg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gzssvijqg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gmmewxshi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gudoonsdz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gntoldbec.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gaysmdmpl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gfmsziqxw.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ghjvllgvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/girathamw.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/glpnkvwjw.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gezhjiobj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/garqctbax.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gcxokmmxe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gxzyqwkwo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/ghmufqgnv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gasazbllp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gfimxkxmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gycsccrot.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gjqyscxnt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gvrwbjafi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gdsktkcjq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gkcxzerbt.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/ganueobmu.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gguetbhwy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gkyzqjcea.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/glgvughqp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gvlwjijps.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gjidrbcmw.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gtbakrzqm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gijpvfskh.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gymihkqbh.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtwchdpak.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gqkqkkofm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gggnhsikj.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/guepupvfk.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gospupvdy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtnhntvrz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjgnmlezc.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gtbiaduwv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gmejwxgmz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gssirzrle.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gakogpxky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gicgoorgz.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gbcuutxrh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gwzhsjjiz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gppgauccl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gxpqvpkje.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gipspukqc.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gldqfpqaa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gatztitwn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/glramidvq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/glotynhwf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/grhytlopf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gnzkfqczm.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gopmofrmf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gjqfxawiv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gjznzgmcf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/grmpqkmai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/girquttks.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gnuxcrsud.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gjotgorlr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfxkfegxl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/giwtepnhz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gtksfdbry.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gmcptwebt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/giqkiocnp.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gifyyhyka.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gudoysutw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gtpguzdyx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/ghfuxltlp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gzspqhomi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gmxvcvvuz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gknqwsvns.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gucvzkpyr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gugmbzinu.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ghncxcmcc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gcshoglyt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzqwiorjh.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gtflpieri.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gcfoxbuxq.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gusvpnyup.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/glptpnxzw.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvrletnqv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gkmuvjgjc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gedvzgmjr.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gkxxdhfgq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grtzpoxbw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grdiczcop.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gslxbvbzb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gqkmlfldy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gbqkjmtdf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gsqoscuor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gngkdvrxu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gdclgymym.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gxatewaxl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxasjkxof.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gjqtywxdk.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gkwjursdb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzpgpqjln.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gataywgvw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gkovtbytw.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gwsipmkha.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtovvapbd.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gmdlzqjxy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/ggrwfrdpq.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/goohtlsno.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gdgnjhhnh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glydrbmzf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grkwsmqua.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxespfyoe.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gukssloqb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcovzkift.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/guqkvjmbi.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gltriarka.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/giseppjqh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gmfowhvcb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsoysgz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ggcfedymp.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/glmqcnmaq.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzxapwuly.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gddonoltt.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/grgaidsnx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gnirlahvo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gryyeynfq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gsjhfnpia.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gtoidniyj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gudvwjtlt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gqkgomyre.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/govdsyqry.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gaozfzsnt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gzfqlkkph.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwzprmjbd.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/girrjvasu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxlnomhtr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gmiwaiskn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gdcutgglb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkmpbdqxh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gamwvezrb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gsgsbdlrr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmqtydsue.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtayunsww.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gcqxnkjik.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gytnhxyas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gfmkyiqrv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gokrhvoud.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gxrwgpsbd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gyufhnsvx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnabhwqsb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gpdqzctdl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gdgnabcfh.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gxbfresiw.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghsncneol.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gqketmgmu.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grpuiwaud.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gjqzmwqix.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gxcjalepq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gaczbsjmw.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gobloryuk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gydbtsuam.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gfujaszzi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/givveesmi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gwmmipqmu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ggrwlssca.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/giqhywqcm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gokraciog.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gqkpzyero.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gbzufzomq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxlgqjdrk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gdyvcwrvi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gqgjaearz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/ghkuddbqo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gubxjltqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gzteccajl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gdwfcsyiq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gzuzhctes.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwrpebhxu.sHtML


<!-- 参考信息 -->