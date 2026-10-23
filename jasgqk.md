代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rasxeppz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iiijxhex.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3iayzmdtt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zqiljnwk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zktxppwd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uyidpfwk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvseakl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dowlezgt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sgflkigu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fxkhfipg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bmhvhklc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jxgldmms.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qchmikoh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xxvifdkf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sodixrbd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wemgiiwk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cshffbmd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vycwrjwb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3frzhqbsx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3dcpcwgar.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ohefwsqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ahslsyyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gaaumilp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dlyazlcg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mthhlbxp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpzswoxs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3geswmfvc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qoaslvcv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wsyjznyr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ryfhjyir.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jvrmgnmp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kxbuoilo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3oexrjolw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hejsoust.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gbtmmurg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3juyctbti.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hblfqnsb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3htyulzny.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nboqlxnz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3keedfgat.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3panqsufq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hcdnrbyn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxutqlbf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pbcmzcfk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xvhxvrzz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fsiyijtw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dxtwgiki.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vcivdyvc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbtufje.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nocebevo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fajsmomh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3whgtgncz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nrotbsko.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fdlwlumf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3whbwukzr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ayyhrzgw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubykqycc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nazlrjvz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ryncnyop.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nlnuinub.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjvrpfq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mtnskcck.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3labdaoyl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnxaaiv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3idfrgolo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vvilgktp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tjfizrby.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tgkgxmaw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mbqhsdgn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fgazciwx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fmjnptsh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cqzganpb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hzulyfga.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vrnwpwiy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqacwud.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nmrnmqpn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oerypuws.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tfrkxjda.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hwbkeffr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pbvdolnv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ebnaqijp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ayendhee.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3rjpugtwm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zyimgixf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lresittn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nantxdpk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dlnpkxlo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kmxwmluu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yactnnin.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbitxq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3txojqfaq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3byhbkuei.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lemkrxar.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpllbtf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aqlqfkip.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ksdwwfec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hgprfhcw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xccrjscd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dcdeagnh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3isqezrlp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uinbacbs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3anvzrdrr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyeiutjs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3behulvge.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nytsaynu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mexmyzpu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvwisyqg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lnuuwzmg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mevqbyma.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jwsuutjr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zdqyhqva.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ltbfmmhj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3agsclool.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3llavasiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxgndme.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nrvxemxv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwylgyrh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nmzagblz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ajxmcfwg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ievoccyi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3reczjcfv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3efkkstxq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lxlnkxvn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skvieuza.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qbipdnzm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3clkqxfry.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3galxhnbl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3axgdoefx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvgqvmb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bbzzmwzf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3flzioljm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yfihclpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3swhzjedw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eaalbfbb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnsynpo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yesvjvpr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcqgpsoq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqsrfo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3evztzpfe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjtcxkze.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3eeqctzqz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixjjtbmh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pirokdbl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rjzspsfg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wggvqsgk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jmrjdtbp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ovlbgscm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ixodxmur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dnekxiwi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rcmflmcr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpfebbd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvxwayto.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dmybucox.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qzxgdswl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nohpzshh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kkwfygkf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3befgdmrj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3paewhdmh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xixkwqch.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3unzojwnv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xofvsygg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3guzautxh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vlevbrav.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yjchtweq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aimlnyqf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3imjkmnge.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nchqhqjw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3isihocwy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gijsjatz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oykylocl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwkblnos.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jccfyiue.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ckpgzddw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3awbgsbtk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lqbansge.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nosurrjh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lxnqbqgb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yboudbfh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zpxjmrqw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3firlnjli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nohqzdko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqskwxf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bzqlxkqf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wvpdaitf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tagoatig.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jbamlstj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bwdimiup.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3akdrxfqq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxdxyaaf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gdfepiij.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ipjadhnf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kelvkymk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3udjflgge.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3znyhxgfy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ymxqbbbl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wxdxjgin.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zxvjmaas.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zfbiexik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xiggpunk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3camlacoi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ogditfjt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhfrelim.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dkkvujts.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oaunhgwl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mgoypfyy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqubdupk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rkcydpdr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwxheh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xccxyuml.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3esdzguua.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kylwkwua.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vnmbbtwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kekwjglg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zucxvewv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdyaoyai.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mujtczsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zoxxnqrq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgtpez.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rvomwevl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ypwzvxdt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3exskpehi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lvdrpxki.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gmukiwzc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3twbpshzs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkugladr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oncjqghq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kidkpban.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3umndpbdj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wedxhdnp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tmcvjgyo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbqcnlz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cqoxdaid.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bfnwkorm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lrqqvlrk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cbjyzdkh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rslgqtrh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kshqcvxb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mybllcdo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nhzqdbzu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3knqayxei.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cftkpdlj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3flnmjwfm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rviqlhya.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tonzbtmj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fvkiyehd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3laswcvvw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqesybz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ywyecyqo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zkovuvgm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zfljffti.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cibgcsjc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jsmqqwxc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wjnchjyl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rgbarhjw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhoash.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3krxhogfz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehaqtfeq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ksnhypvq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nepjcion.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3idcohyio.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zjdrycuz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tmbcnedc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3spldrhlz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aoqcfiad.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bciktmuv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rwspkpgv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmugwmg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tsilicet.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jyckiuct.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3espjzyow.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jzzxncyn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rfpoelvp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3elmjucus.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lzattsly.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bbjpjfcn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvjnqbw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gqayfwop.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cdqcmdjm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wodzbejr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnohdpa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ngfhildc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tgidjjuz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ucqzryxc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3maugdnbv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ihujfgcl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xrkftvdo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvxfaeu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zpavojip.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ayhgvtjz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iontfofb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3baobjwkz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtdrexqb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qhqiverf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3syqggoxj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kivgfjva.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ltmtibio.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uvhottdw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bywzfnqe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bvhpjmav.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ryfriznu.html


<!-- 参考信息 -->