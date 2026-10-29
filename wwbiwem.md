代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gtomskwej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghydvqlxe.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gyggyjzym.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glmefwpno.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gzoodzvgf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gxwvwmcgv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gzvjsvnjh.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/giykviget.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/grsmdjjtt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gffbzpfjz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gihhgrztm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gnbzprnak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/goquywvcg.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/glharrvks.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gncmsanpi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gevewzlbo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gjogyggme.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gknbgpbsr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmsdteuaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gtruokojm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gojromwvd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gcuwihtyl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/ggxxwqdyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/grxkacnwf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gnrogfbzi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gczamvcdp.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gujoruxoh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvsdggevj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gpaybsrst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwvbbsbsh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gjqswkylu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/ggnhkgvwd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gusywwaif.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcyudpilj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/grfhzkwjv.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gqudlypuj.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gglrukxdi.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/guoreiiba.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/glehsnirl.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gbngddwwr.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/goaxcgveb.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/golpxbsnw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gqcncprzj.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/ggyvrysez.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gyofdnuqy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gjrxqthqi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gvevwocov.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gaobtnxse.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gdedyucpx.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfcnjpgzc.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/grfnylbfi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/geaiumxhf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gubpiynjg.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gardvxbql.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gwbdzkcci.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/glrrathuz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gyjzvifst.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gznctkpip.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gzmdymfut.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gpnpsjqls.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gwskmenkz.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gonqkmwzq.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gldxsphpd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvyqdhwqx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gcqpuoesi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gglzxeiku.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/ggbftdgxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gulwthaal.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gybnnxvip.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/guxesbomk.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/ghjhefjid.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gtysxdbvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gqeyfpytz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gzalpoxrf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdwevfonr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/ghykupaaq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gihrbnxpq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/ggkaxbluy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/goddejkcu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gxqfjjdsn.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gzwunrpqy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gtqjprqyo.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/goqsmvwhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/glkwbfqxv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gozygislg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gtbzblotq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gberjpbzf.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gxqueseyd.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gzbakwsce.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gncbcztcc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkwgwkryb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/ghihxfxdy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxnuhiapb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/getgivzjm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gllnjwbeh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/goxspgwrl.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gqyqurlpv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gwndlsbqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gzjvrdvvv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gpiygswgn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxlmbvlqq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gvekzjwxj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gekldvlzh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxgdkujyl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gkqpqdmzo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gtzwjpbuo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gpbkiqkhu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gqvjpxdjx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gvcpjjdhe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gesrtsaos.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gvhlipaaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gfaqnvtco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/giwnttmuc.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gnwslzupr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/goqdhocqd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsqmeudam.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gtoaqsrvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gkgcevrga.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gewwiohug.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gunocujqs.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gmsblhukd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/glqopjizg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gdiqxcscg.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gubkevexp.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gasyydffs.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gmjfltrfo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmnwgumra.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gyvhvalfv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/grjqbqiqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gufgjuwcv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gphrsibiz.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gdiahciqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gwooantui.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gbjomhrng.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gzykmyowx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzpnkqobi.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggkjqforp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnmynaflm.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gnwcpdflc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gdiserwag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gzbrbfojx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gjgaefqvi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gbgchnmsb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/grzcmbvlm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gwgozbcmf.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gaubxukxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gtjovhsru.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/glfgollsk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggtnqreau.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gpnvaamqd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gpzlriwjc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/geuiwikyf.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gabscxjhd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdyrwos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gvlzzdxpg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gkxebhail.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gmsebdjyo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gzsnwzyaj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/giebbagti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gmbdvhahn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/giorjiujx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/ghwasjjck.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gcxvsvbsh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/guwklumni.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gopfgkkyt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grknqodii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/ggebxgirw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gxeldmvyg.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gkypknrjx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/giymuatjh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/grkrekfhn.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gchcmpzuu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gnhfhrrms.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gaaaxymin.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxdgozhyb.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gwddwrdvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grmtbfnqe.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gyhnjdmjj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyzvozfto.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gdlwwpeqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/grplwvddv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gbioaeauf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gtaogilkr.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gjhayjiod.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtlwkacec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gshpwzjia.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gydxnjvsz.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gznclkqel.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gykamsgza.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gfeaqsyqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gpgzgbfwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gyuzkfqfi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbfrijsfc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gxadbdcop.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gpjykhewn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/ghlpifnqv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gjwbttbwk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gestqrbkx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gqgakqyhe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/ghtvwedcy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdmuqtrkh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwsguafn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gnmhdmssf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gbgssgogz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmnkajpls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gzvqtxldu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/ghsjqhiib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gchpswfid.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gstwhpyxy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gmglueljp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gvohyigrs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gibpcghbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gxhhwdmwp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsmnvxswg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gdntaxpek.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gevoajluq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gatcfjxkp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/grmcspuzn.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gpgfitvxe.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gsixhwowa.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gqhaldxdd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/glsavjzhj.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gygyjeejy.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfusefiq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gscxyxjbo.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkkdjamtz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcsrkkazk.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gxolnamnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gqlpfcjbk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gpofrebfd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/geljljbhx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gdjlxmqda.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gdcqwhdkk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/geuvvypks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/geojheznc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grqhjdmrw.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gfozhwtfg.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gqgohhtsp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gahaowtjt.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyrtodqqu.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/goxbtonuu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvenezzdj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gglilifcr.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gnpslgkhu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gtwjvxuoo.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzdysfnql.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gzgsabbbh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqdfyxlyd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gejjptwcs.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqzitfqfs.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gcgrhpzvx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gbibxtfsg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/grtqxvxry.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/geaxjetcj.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/glvrwuknf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/geekkliyq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gycgdhpiq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gabncsjkh.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqmaufhye.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgaiaabw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/ghmwtxpdf.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gjlvgmrng.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gzrehtuyw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gwenqqnzm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gzzkssyzv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/glnguqros.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gtsihyxoh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gwdqfyawc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gajllrgrj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gkanguerb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gwmdtieyo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gyoljjdfc.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbcxcteqj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfnulvjix.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/ggezuptup.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfzgoiyob.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gniolhdcu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxjzdohrz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzzlzhiaj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvjqmvlkw.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmshtqvpv.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gzeqmmlni.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gtibnyrqx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpeeohffb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gvmlpgtoh.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gtwpaxzqv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gpkdgjgqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gcakpmflu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gqkkawgvy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gexjuisfk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gclkddyaa.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gnnrwxsyg.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gilqeqxmo.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/givwalegf.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gpqpnorao.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwcwomjgt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gzpvauciz.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gyfxepmdd.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ghoihzddw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gnfhnhytn.sHtML


<!-- 参考信息 -->