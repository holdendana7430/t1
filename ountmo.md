代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bvwtngpk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dkuyfovg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjmocgbp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3njlhzxbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xwfmmvgn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zgmpbtbi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odyeqwle.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kbxpmnfp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3abowcdhg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ffktqous.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfwkagqq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3arscloml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3elpmrbkd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bxmwzpgc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kibqcvgu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fqubmfpc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vbkjbblz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cktqgwlf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rndwzkll.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3exltkalu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwsnofcm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iujdphqe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ryyyfuyk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ustatzsk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bmjffpru.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxielf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gruokuqo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ygavnmkw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ywviejju.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wztawaqw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zirsvwlh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yjolnioe.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jckgauvc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mjmubmec.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jjvhelqy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eyhvajqd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enpiovvl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mnkmwrjv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fblcubbs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mfktreti.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gyvjwznh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bxuheayu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jxtbihrx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3udfjzlxw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3esglqufv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kuyjbuem.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nixbokuw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hvkdmtkl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pppiauzk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pcolsstg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yoghdfoj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rdkrhlqm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yuesubic.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nugwbrbj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ifsvumgj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rgdfqknm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uekmuobo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3engpilil.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3blegmwug.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pokrzjih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wnfcwgpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3soagscyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvazszx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ydxvloae.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxasapdg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yxkbytov.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnlborqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ulsazroa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gicyrtzm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lpxrtvvn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbijtpgl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hhaurofp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dnelbauh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3szxhotqa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3iaibuuvq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ruzdphkx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sehtosrq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uelkpwtx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yqvlodpt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlejkckd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoswstrm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3orvcywrd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mmtacwcl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ibkzbvjl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vxvaooiy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfucdzq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrnmdzba.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eeaznabc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3weafukby.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3htndwrgr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xiboswdb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qhurymzp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ejmhbwoy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lxvwrryf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3piqhztvs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imjsfqix.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vfhgkdlj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3salkygly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ayhfpjod.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tnqrqyqt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3smyxslwb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3espprdgy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emociqrr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dkodvpom.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3puyjxrro.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zcxbbavl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xkqhgqbb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3adntzzkf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yeysghqy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3depfnlys.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enebwwio.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fifnkelo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ltywmzms.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sjibiply.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uolyyqig.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ppkrdxvj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nwavzrvo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sccefbdv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hydnjafy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkayuca.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzzxhnmz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wmwqyqde.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qpxdcfnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fsdadgsx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3itzpwmyg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lnnsovum.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vbezchex.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3grhxtlfd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tntozczp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vcgonjdm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dfvjeukp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dxbbgwpq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3imoknfgl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3avttiuiu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hvwpxodk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubyaxrlo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dgdznjob.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zazsqrpk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3twblgtgo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3cpvmbpir.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dopxszws.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fkoghoxc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gspwzwen.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzlzkjg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wimdeayu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kwaoocls.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcyctgoy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yljiixea.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rqgptstn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tchncyaz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jzqujvvo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cdgvhniw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zxuavvpl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vqqlzrxb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zabllowd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wkqovxjw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zggewctk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vvoekuhl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gbbrdvnc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ojwpjoau.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ejjcesqs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3txxkhsju.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyzmjoq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3giljceer.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxsupnti.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ulvcsopa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrggzttw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hsigtqbv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ljsjaspb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wqaguakj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fecyxdea.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kecfekfg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ashmwzar.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3anutgdiq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykqojqrq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rojuccrp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gbqhgsas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcznmvg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sijxcksm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sjnsnhim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pkyhpkoj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gzauhxre.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3leceyvmc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pceiheug.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3boeutotg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3etxjqvrr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kwzrrfqu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkyyzttg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3miymuqsf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3veyacwiz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wdpyqwrb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3btjpsyuz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3deimturb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vkafgvgd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yysdrjuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3grkzbcop.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pxjfxkaf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loszktuh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhqogmcq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dizzzaix.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vytihcoe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyqxxklp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3htnbtpqy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dltazwro.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhculxco.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wgiwokwd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nvoattzk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ysyaffwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3empzcblc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3okjzuhxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmqcghrc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3npzxfzgu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3onvkomhf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xqmxafko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kmxtnaxu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bquxvqef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3arrgczgh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmqkqsdi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mphwrvsx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3joegguhf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3suqweaef.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jzbpmuev.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jmmaiocw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfsibjqx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xffrvuoe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tffigbeu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aistgffc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uaihyfss.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gjwhcrlg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vidvmixb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zysfahpz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eryysywp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqplcmj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gaowfrcj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjinlta.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wafxbrls.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fmwrtbkc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bbqtpmpg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uzusknuh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sryenkkl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mejjqdkw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3swzwjdit.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gikiatez.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pmholvem.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kjdhkrso.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rfhowbuv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ckslqzvc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mjxmxbvp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vevclfea.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3encekymm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pdjrhoak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aluimqgs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kktntvfs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zghtqktx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xefyylti.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jpjitguq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kizfrwny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iufrjjyb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3euydxxfx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ajiswqeb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qjtabklb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etrjyets.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ifbftzqz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ullnvaaw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txuxoawn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3axkfvpvo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eurhnzrs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpquacdl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ligrsffg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzmloum.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qvreghyu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjfeaai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kvpziuyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmkynib.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3owrzasna.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdudbmw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3glwxtcxw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wzikqzqk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3digqqrlo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cghpzhlr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vzgqeuji.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ddbmkibm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcquoun.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qecfrosc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3seifznfn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3txwggobz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ycsdincd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rtvncsyh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3klipfmux.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ixbmxdyf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dzavhtdv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kydykfyi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lduwbaei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwevxr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jrbirdbl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hgwqzgjq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3umqiawbd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xysdkumy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iuzletuw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tdwlrkww.html


<!-- 参考信息 -->