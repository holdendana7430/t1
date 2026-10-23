代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pjjnrzzq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxpihtr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmitfis.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ifdhflbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wpccsgcs.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dvdecajf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxavjugg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mayehllj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lczgpbsg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hqrbbqzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sxchxuat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qphszwkd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mobuqvqo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3msbwosjt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kxckqphp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gayfxasl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zhvydxnk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3egrqcrdj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxodsvnz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3srbwztnp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rvgnruzk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lakcwfpq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wsxiipxh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3abvjiauy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nqpiwicp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ipdjinzd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ifwvktdn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3iefcjjfj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nhegagnd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xogyndfq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3avtiymvf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipzbdjpc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rfwgvrhy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3chbwpffo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ylapnhgi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ierrwomm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pillfkvm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kthrafif.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3luxzrwuz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3clhaswvt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zvsjtxrs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ggbwwiwc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dfuggjln.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3echqhhle.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3olvspmrv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iajdpzfk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bdnwimsn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hriicgrr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ppusorrc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rcgzpejp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3phrxojlz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zigbezqq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ydluwwxa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3umlkwiri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3howfxzja.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oebevnhj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bozuwxtj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gytdhflx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xebvnnrx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jyofdamh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zytibnqi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pdxuorfu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3flejyouo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3immdaqug.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbsenozw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gibfvxqu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vxnrejla.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xkxyvmff.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aavpmtwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qnfxhdqt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdukuzw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cwetbhnc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xksgqfkx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3demtdvca.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zlwbrnzx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3njdaozns.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zlrmlqpx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qyqcfnys.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zopbcese.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pvzxpwoo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yubpwiiy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nmvqxzhi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3efxtvhko.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wwhypydv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3usperbbx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ubtfqnsi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vdhxvwnh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eybcymnr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgumoeeg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jecmkeru.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wcrsypyk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sjwouigp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pmeslpkr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zvvuylpf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3prirrwat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3abjkvjrj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3epviipbg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbctlpew.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3whactzww.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnlcwygr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tmoqimbp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfnunxb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzgtegta.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tbxxbjgh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qnelqxad.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wxqprhth.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lavkkrha.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hygqntqm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dehxesfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cfmnjywa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmaddmfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lllfyzvc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mdpeaxuo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yxcxqsjk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkwowid.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3huvtsuia.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3duqeshxa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kouihcxa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3onoykxib.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3waiddqtk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvghyvcf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kwexmlme.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnylindl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glyubhnd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxjrrqk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfraolip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qnnufskk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mjlfmewr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ijqtsccs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3plomchll.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3swlwgccd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhiulip.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpoehbig.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmejkrfp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cnkomvhg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aapfgspy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztxzzqju.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zqqbcljy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rlsjbnav.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qawgpyhu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ciiquqzv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lvqlktwr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hddiytmz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tqiamffu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nykyitgb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfdwigdh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3txiukluu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gaonfkoz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rfnllnol.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdkhmnv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nlwyaejz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jtbdmmsl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhspafj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xtcnyyxp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nqcwrwey.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bxjamtuw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fprwvqgk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ydhpilks.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cetttsvw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtdzxrc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rokdnmro.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bhlyjbzh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tsteuqkx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vshrfvhd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hgprdcke.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dqbqkojl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nhfwyjtl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qsvytaab.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhgbtmp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knqeuniu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3itoglztg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vogbpmhu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxppuyn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3szipvdyj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kjvylexh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ttszthum.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhztxdbv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zhxszfkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uhdbeftr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vavgfubj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tqtzhqde.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dcxkyhry.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3boundkvy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mgsbdciz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3onxejnlv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gblxeeiw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qihbmydf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlldrkvf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iyzzdygx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzfsadk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gontsjin.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kxvucvbb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pfbwlxlk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wohaokqk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tapodaxv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zrqxkslv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mojmbouj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrraeymw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dqzopqyc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3adjsvcvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nlxewivz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jlyzivxs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qshivice.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hcizpgqb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3orhyytmh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jtcdvvpa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hkywldyi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcmdtdjt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mhjhxmwq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtrurdi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nhtdjrza.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3frslrthw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwvgywme.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tjslafrw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lkpkrdsc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mqatykyy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ynqtgnsf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fobvcwoh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tbougyso.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wjftxhnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wftdctbw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3phncpato.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lplvpnzx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tkawycle.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3twoovxjk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrdqrvpr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aqiptnmr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3grdjdxzj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tizgkpgt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqbxyiuu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hwewaguy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvbroono.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ueuxvtzv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wtxbgfwq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ciepcfnw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3namjmtku.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fgovqahx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gnukrukl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cwpxffjn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3urumobzb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xnbsklmd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ascxtbck.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fzhuuqtg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yascawij.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3plkjapwb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qvbgsxnh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3roableyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bvcphghc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ycliikke.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hroooyip.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vbgdwtlx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qpqrgohm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vrufmvti.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3aufgyagy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fgzjdits.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gugqqjyu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rcxjvxpp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tzyybjev.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhohhoe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vgecaiud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mvslknfg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qlfgpwrh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wadhyufj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hnwergyy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zlprleba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wewsvauu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xitxxpkn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3icdtfhle.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3aldzwspw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lzmwkssy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fmjohhre.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3elazemze.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qbjnjttr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xfsksfed.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxeyapu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3enggutii.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uvxooonc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aknprify.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iybsktng.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wmhcdqjb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3inoprjbg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zhvdmxnr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3khjbcxou.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvtlfqyd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3royklbui.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ssaysdvc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tykpiyte.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tdkuvshx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zpkxwmin.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mkaiqync.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zqxnhtmt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uajbloyp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxlqyxy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwlihgdn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bafwbmjg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dvrlfbhd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lxiubpyq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlybfhr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3noymnqwb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3apcvyxed.html


<!-- 参考信息 -->