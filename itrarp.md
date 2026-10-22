代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pjdhnbyy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jikxubrv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2olhmvbgz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mhvyyuie.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dmondbmf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbntpjdj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2outcpzda.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mabnlfzc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpoyavbq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wmmcngej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sceljyvb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujlhxqzb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2paprklvh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ojleocqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hqzixpdv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wblikfwh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkcbbyd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dxjdxoyi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxdtoujn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oqpgbbca.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bhnstqun.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2idpsytpz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jkmzagyq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2davjvxed.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2grgsdhrz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ggnmpbyb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xtdltbsa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qqgjvszk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rstovzon.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aologaym.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wymxwpbn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkxushrd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yeccokti.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vweomwrm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zkpmptap.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ccioujzx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uqjnfgie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ijnzqlxb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zgbxvjgi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qvqlddzu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nziqiwoq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zidmbeeh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wzoasbzc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vnentbco.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eqatuoxn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2humemplu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uuklamtq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxqpsl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eybsfhbp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2elpommvh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rtxvuodc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ziidarym.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nifpenll.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qucffsff.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mrvsuczy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ghlovjmj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktuzoykw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ydedxxth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mjffwohc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cmzwkxce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psqevbuy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2anffuxho.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rxyiwnju.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2krojwnvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uyohenjz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uqparhsb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcbinls.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxxzcyp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ojjmbcoy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jzyiajxj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwqsoet.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cvrlwggv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tvcbbvzx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yxutcgkq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrjjqjic.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oibqygif.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ppprsvqy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nkfmovhd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jerpwylv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iuxiwzmw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zncqjhad.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cpmhyvve.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ymgtytvk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mxfoldzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2thqeqwcz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xuaexcrc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rriaeino.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfdumlpc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vukfgqyj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2snctopvd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bweckzrq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kbgnbcjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2npghqade.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bplfzrzd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2icljobjb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bbyzvbzo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ktdyirmq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2enhnjzyh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2demwclwv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2annewboe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lwjyelef.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikwvfwjv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgtjnoqd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2idnewoal.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ksbwsfff.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zcuaacrf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2itfsaazx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhlwfdhe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sxiwwzqa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2alvwjvjr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2joudjtrh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ditrsbfs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xyhwejns.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wosruwkm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fnwcxlxv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zfxxitqy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lkduuzra.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ydntpnob.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjduyuh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mbfvfzhy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2raldiysr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aieaapwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cbnkenxn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2byrrczoa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vmdyiedc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wfifsszq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2belesftk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mamhfzgg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrzeln.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yovmpszk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egoolhvc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nlyfllyw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xoeuwfqn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2albzvkhx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pouuaden.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gjgllyie.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rmcahycg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lnrxxzuc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nohvwboe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qnumhcvw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ijslwrsa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgkbzaoy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yhqrnpbs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fwzbtchs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yscmxnrf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnnrprby.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2bujujync.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2azqipwea.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iurilidc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hnrmitih.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xmuvjtxl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bduovmpn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wonptiqv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mwyxmwfx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbgkink.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hmrvtmuu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lmyivwgy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bsveejli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uwdxprfe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ydpvihtr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2elbhyxed.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bjglbbxu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tnqugawt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nmaqfjac.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qdlkraad.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxafckkz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtcncci.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xnxyvgty.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpjktfbd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kvdrlctq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lqdeodnq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vzaofdtf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kifoaavc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2sdbssloe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atqntshl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2nkdardnr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fvjgxrzh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rnjortyg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cglrzsye.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bjjcgwoz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ifgfbnia.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2amryehcx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2knpawcmz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2emjqwlir.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2awnurxtf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2roosqyzg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wcfzlige.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bgeuuuqh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pjljfuwr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2whjgxngu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2apcrjyrd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihicoobz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rotkwtth.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhtodoxk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxeplcne.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pjmoksrf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2oqdbbzpu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wkrsnfmy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jkprkvzz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qbgjcvoh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vtufhsyz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyhxrle.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ckvphhgh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ezxdiluj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qtxeufnc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bpnullhz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtxlccps.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2sawajwdj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dlpovwmg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhpcxur.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2khpwxoog.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2reydvxst.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bgzpjmyw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vsiodymh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bluqhqbn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycltoouw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dosqsvye.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ockkeilz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxzgwkuc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rskxtzrc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mqgmopia.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dguyyxfw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kxvtuzqb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cxldkzzp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qwmhyfwi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zvoemshv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gftonmoi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jjldmwba.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fftozlyr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fwfmtccd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzrzbghz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmzooh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bvtghhdg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2knkppqyd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nyyyzvzd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2twpuclpd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2euxfiedc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qwmzjflk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zhctabva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2umpdsgbm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxyumpiy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibkophwt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yytpbjey.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2debxazku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2exygfktc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2egoplfnz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fgaluvuk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cxvmnmly.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2uxudpedm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2anvnvsba.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxuwphvp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dpmhwwsl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2stszctkn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gljwggle.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jnduuppu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hqcpthop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cyapgxip.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2uypzkksw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2orepomcv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkdnvbr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2popxstlv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eatwnxys.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ualfwvft.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mecqohib.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vzejneaa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jbbhouzb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xyreddrz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rcpnakgy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ihgeaivl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhppmzrh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtbfrji.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tofyllcs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vgunrtma.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ylanshqy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sqimmpoo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tifmbrlf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sgqpjfem.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zokmpwga.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mgivdgit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aitbhorw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hmgvcyts.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ungshulw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qknrjfsf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2swkdypts.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2igkgpbzq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uiyxpfwc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vpzinkda.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iigwltnk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxiotst.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ohmiswuz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fopmjycm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nrvpbddm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2iykrhypc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fegshlch.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzhllf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gwciznho.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxkoxlnl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpxxktei.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zqihebxd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kqiwdepf.html


<!-- 参考信息 -->