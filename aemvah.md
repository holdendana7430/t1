代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvfnarh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lppdfytc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjrjqstd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqoorwsp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qjmruvok.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sjntpsva.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eufqfhdu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jthudodi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fmrhzuud.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lecukenn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ifnugxxs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wqtzyrqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yydbrsil.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fppdftsz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wuitvrhf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dufeeugt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3enjpgzcs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pvnefgpw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mancuwwb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ofpgjiis.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lopcxckv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxpyobbm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ovlmwdmc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aroazwmm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3guqcpozt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gewgrmml.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3soamxmvi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cnebmbmc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iuojtjcb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gttqwjxk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ombrbriy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfyqequz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zbnajfci.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3llbylcej.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ckrupwba.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aetuibzb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jtcenwll.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqzjwfbb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ddgoskks.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gufiviaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zybhzyaq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kokoctko.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbgvktvb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgcbvsq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jnhbbmmz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydbhsndx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zamszygh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fxkbhsoi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xyxzswyo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vlvitogw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gdyffvei.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pmwqsbpf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3shnoelji.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bjrykkdf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ixuhcgxo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zweusdek.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cwxkcdoo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3decysbmu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jsweiriz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pdtarrji.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xtexgkot.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kilnntfn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qajawjsg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qfznpavy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dafhewuo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xbgwyvkx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkoegehg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zbghfwki.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qolvhlmm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ldsmaigf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xmbmvuwn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cvamuvcu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ffykwtrs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ageeekgx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ifobodoi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnnsvfyz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xduqwxyn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sosotqga.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3haxcvmmi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mecgakll.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xzotldqq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cgrrridf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xlqspyfw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kajmximz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lryqbjfj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3icmzhlzb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3koklbwbk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ddndwgnh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kptuslko.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbnxxhaz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jsdwqhbf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ifcqmzgb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3invaoogu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fzisipsu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qfqpfcqt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ebkakmpx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olgwqrtc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oyfyhxgi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3thruesvw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3phyebdxz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dvkhpnzn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qivrfwju.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nxartlgw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uliymsmy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lgzwcvvx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dwanjoln.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3luycfdov.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3djszbndo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sgvqijbv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pymczdbk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dehsscqg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3icxipfep.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqllrpbo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qpzmexqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wzaxnuwy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iokmzgwj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zcjrhuzs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3aslqevvd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wsfpvfzf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmyronis.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3snhpcnll.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvmseytg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bunchwkz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ynupgczq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bshxjgsa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wnufxmgt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qljdtsmk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xgicvvbs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rugxbifk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sqbuoxcf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rslbwwmy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qfswujyd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkljkwwo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fiutmmze.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3usiityzd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjeooc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3focetder.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lvmrcbmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xspitmcq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jlahwqvu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tbjsohgn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xkvugndw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3muxxuzho.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3shrulryc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ljqcqdoc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rffyygbx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvjbsxl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukahyfvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lnboytzf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yyyjpsih.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tmdywjhi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pinbnivh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gkgiqwgy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vuiwjdpn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3znxajutg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tbkgrimc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rfhvgrxv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mexyovwq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjdfiyyx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqnglrjm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3czeqtgvo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnxulgw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkkuyqi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ptyiuwsd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzvydsy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3thewvbst.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zethzjlq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3umntfdfx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wzeohdtr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3exvwtqvy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qmuiujex.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ytzruhgb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3eoaysjwl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwazxzy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vvrumfsl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnfyhmy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zunwovqj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dzmafliy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hraolzfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3odgkvecx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wmcyesgb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kxqlxidp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wcjfhjen.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vjavxini.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rlnajnnm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3taembstz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3leksrjtk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pxaolezn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3feerylgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dxdjelde.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zfhliccy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ivzaebix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pyyuglee.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvtubcl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ozdpjxcj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcxzyay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dphxkrhy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ciidlecj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dlijmhea.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xdqrjfam.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pvjdhecw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eefexcey.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3paynzddb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gwxwulpt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3poikytab.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dajwkcsg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lygqomfg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eyjptdhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omdzqrcy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pqzjytgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzyijvos.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijghtlpv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rflzzbcw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bchevayu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hvqbtjib.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqjecqf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vzaaejcb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jqtwvpez.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bzhxveob.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwvsskb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gklmuqgt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pdlpyggz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lcnrwsiw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3damgacai.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vikipurg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3owpxvtvf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3snayvrnu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jlozbdzf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qalookrz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nuovdqru.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bfgroaxv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3avtpqnyr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qncrbqho.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhqxsgl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hshiswyq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wlnzgspy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rkgaryzb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdffpqpn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3sssaamtd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rsqxngvg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nkwtyzhn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhsfeky.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lseyixke.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jotdnprj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhnoomgz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3savgonky.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mikgsuwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kuwrekfl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fqxxlrdf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mkmvyrtt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vggxasqw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3defcunxq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3whieruzq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vshbfqka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qhekcepv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sjpdpzdp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wgtbtzca.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oljnzodc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zbaqjoor.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vedxddeu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bxnolswu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aahnzifg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bmkhrieo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mdycdnbd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3teyastwc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zaxpnkxi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3woeckiyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvpycpnm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rqgqqlmp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ugxxqscv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3haimpkka.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qozcjqos.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ofucnolk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xbicuawj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iisvslmj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3chqdvduv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sialyeoh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sgqqhfej.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbmuhjc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3erkqboel.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3foqkucdv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xhpcxgof.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ftebkvru.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lswdcool.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dwbchghb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3karprwig.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stdgzrxq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pmgjxuhg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cgcriyzn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rxxzldvd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3erckkaqr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hwrxgpxu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fbtuiape.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3magwhrpo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zqddrbpz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3olcaaesh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cttnqnki.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfpzrlr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rdaxwukn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qduhhbce.html


<!-- 参考信息 -->