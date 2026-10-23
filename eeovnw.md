代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dxhfpkzs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wfwdoyfo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3levioblf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wufsditr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcplhgup.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gpkkarxj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbhocih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxxmpdf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iqhrsjoi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3etrvzapp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bniqixzx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psvqszwf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gyeqaqcp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rqnqlhih.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhtkgnrv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zlnbozsy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jokxacop.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jsimiokp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ngeiqehj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3clgkrxye.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vkbdngcb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cwtyacsl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hdqgneyj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gboaheop.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jgtzhlwm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pspdfzjs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iugwgmpa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qjuqjyuz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvyabtim.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvwxwwlb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xvwyonbs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zigahmfj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ikpwfkyk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tujqhqto.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3brlnupxh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3elxsnsuq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3eehrlrmq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uwoczbmo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hjnourxy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dfmyvwkl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gmqnqoep.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgsatwec.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kgudhemv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qghydrrp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3owdckqes.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3korldmzn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3joxluulu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mndazbfk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3iroykauw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ekwexzbi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxkksvic.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qnvqukwp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xadlnzji.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3stpbrjyg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dwcyzakn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3reapyzqq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3davaubgo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3usidjzei.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3aeqrifqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3drudrokl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugolxjmv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hcdbemvm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ihaxbnsr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3awfatqxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lbbmnhbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcgwusiu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3goubipjc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xanggudy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3atcrlegb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zqoffxnu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lghrkycm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ohnlnzen.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dglwfzln.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3sjyxeqdv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wogpjafz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wwrcxrgv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qstvwwuk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dvscmsju.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmjtlex.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vnitreaf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vorxouoe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ttwzyyvf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wwolcjzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oveyaeqr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qtytshzu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3umlubvpz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bvmfcilc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhhhlscn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmagifyg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3phlqxyqj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qlhaytmi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wygvzxqd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kjehlyow.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gpiycrmq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwecqqp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrowkch.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kjvcrezq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3nswfbdkk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3umyrwucw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cobatvlg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wmqytukb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iqamenhf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nseufvhn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yuvafpol.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iirejrwm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mhnrppkq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hvbjywpt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oitrdsnj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3obzpxsyc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zvqqzufz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsuziie.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rfhdkkim.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jknpltcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fwrbhfjz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cfiordxt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dekbaaoe.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dkwvkovc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jdwqlztt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjbdmty.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nxwvlrjl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ytkgtamy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3asobfycj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gsgwogim.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3errgecks.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ektgrhwh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wjhdmrxq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zqcwlfzq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aiuxcaiv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndwuiujb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iozwttpb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3morokhlb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zqubhnqr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyzwdu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tlgchuln.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vvicxwbp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uahmquhi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ormcuvoh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zkyayxcs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gmzbozjv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zmbvyvqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3astytgxz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hemehxqv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vguhboad.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qrayqwts.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pnwaadvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chtktzcb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vmalnbbv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tbzukcdi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vphzghlc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3evevugqf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3izuyjfds.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qggahniz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xlxrproh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qcudfwgn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzsgziy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqywced.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3elgukbok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3spnxpfpz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yxrvhlys.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xrhqkycw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gbosomxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qmixgdlu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eweuwgxu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mtvqqvjn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jmvswurm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3faskckpq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cstkbyem.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkyewtdu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibperiat.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rasgafzs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3suchhzmb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3haruradf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zybskngt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3btdtpdtt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikoqlumr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jpsuajuf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iswfbjyk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tywbcjpk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nrqgjktl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fgpumyvr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uoqslfeq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlqvsce.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ivtcrljj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhjcivs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pctoacft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3yhexwbzh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wplqaspa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rurmahwk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkqzycbr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zdlsxlud.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pechydjy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwfodl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cpynmpwp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3arzkthqn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgvgheaa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yxixzixj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hjaefqvm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ffuoanpn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kuvmhqpp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3msdnxngr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3epiuimcq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tftgnrxv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vanqpwzi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fttuzywj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dkxbjdol.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3blhcndma.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptlqrqhm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yaghvtfn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ocaawhsc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxjobcrr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uwnazvlu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjknmos.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3otalljpb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzkgosuo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3thmwkrvy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dapeebgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvkbpfjt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hcqjxtyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guqjbtkq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwfiogxe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jkxysjmy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ubkmeion.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkbysxoc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blhtsprw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qyypkjou.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wpzpdurj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ixkfeora.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cyadexax.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zyevketu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ybggncqa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3yjgvwxws.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wexoyiob.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tehlfjwz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xkbyrhmc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tzojwmhm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lljfrsmt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hafaomlf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mmlxkalk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uaxsxwpa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dqkduuio.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncdpdswk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncgcrczq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojafejeg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ieralkud.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gmhjucnb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuenxmv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3yjqboauz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lwtsobnk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3csbbkpet.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jzndrvou.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wbybsajv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xsmklztr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kkygsqdn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xvhcdjdb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3geibcras.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tizibjtz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3awxgapop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ganmanai.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qltaodef.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sdlsosid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzkvypri.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3phuukabz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3abrvqzfv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhnvuhv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qqakyequ.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjinlywn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpoupngo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gfvsxnpp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xeklbmub.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cctgrgyd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tblgtbsc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hvdzlqgu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nftkbrkj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3boovtrkf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ghalnsue.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gcompvdd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bfmpghqr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gbkfopzn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3makaiabd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvldelz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ffflsjrn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kfeopflt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xfglfrew.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jgrwmqlw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vmveuphg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmjsymym.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tnjdppra.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3soyrgbcm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jnmeqmsi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3azotpnae.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxtcsbs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3smbmsgqg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3emrhcfsm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpzyhcjr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fgvcqhuw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vknmgsfk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnsmdwfn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhcodybs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vppwfvoa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3opvjkbnm.html


<!-- 参考信息 -->