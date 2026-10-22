代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fzbqncad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqdidnur.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hwbpmlcf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yvnmnapa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2isfytiyg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ginschrr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mdobogcl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2purvuftp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vbkhmevt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kptoprfw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2neuoovdl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2psnibitp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nrhhlhlg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bbrybftf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yqrdwsty.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vitdcfbs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvdmlpdj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxetiib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ankzibya.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpverrhi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lhjcsitr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2juaantpc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2iftbxibr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ithzlnut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pcifzqsy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pnsvxlbc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jtxejxzu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uqjjiqjo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mawzyqrm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zweyipzb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vkizijhb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bmamdnhs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qhypxqvi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xgbsobqc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2axmfgxxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2elllldqn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wtcdwiec.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2iioebqjn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2blkidpfr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wptuhmxg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rbkbyxoq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wjlrwqjh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2aphhngrv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jwrbzsap.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nfqjnzze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xzmixefn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ksficmgi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nhnxjfhd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyjhiwkx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2shqfeylx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jgqvnjxl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvvabcwv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wfpdyklq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewmyjhcw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ahybzukd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fjxhivxn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eckzwpcm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pdpfrdbp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2brsndlvo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2futgzxpy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qpcskzka.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gfqpozns.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dtvkwcua.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rrbfuzgg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ccbvfrbi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dthnpjqv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxavmbx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tjlnwure.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwphihl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kzjyhdjr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpenrwsc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lpigwkqu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzfkjdqz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hygtublw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rojpwpdc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jkdqcvij.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmlcvajv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kvzhnyij.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fwhhahyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xgwxlnun.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvgygft.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hddqswwx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2afmzapqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bduubzph.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fvaqeyev.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nuysljcm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oxntxibh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2slddupsx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bzgbgrue.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gtowpzyy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kyrpodjz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hovhgsde.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ioyayxwz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oxlaewnl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xulzvmxs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2idmvnlvb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wzqzkvmz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2exlztdrx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qupynxvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2itrmkido.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2haiarahs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ibewgfic.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yqtwwwcx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtvjznjo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xzeobqmw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jddsrpml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zpdzatbj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hahbacxn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fygnsvsq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2khzhtuue.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mekwllva.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ociioane.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2reiaxnxi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nskbmytt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtoeocl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vedbtsoc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qoahcajd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwbkrkki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2frytadms.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2szzgpxxi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kdgipivp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lzznyskr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmhrutg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngzoovwo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pgfylwdi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wrphwhnf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jntaekhp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ldkbufwp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wzvmctnt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iiwkiypv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aufcxqnp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2evxtytvw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ojoprfal.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mbdjkqhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2udqdhxfn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ffhlyedf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dctifwrx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wrgatqap.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pinosnoz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqtdzbqe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bklgpkkt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kwaytkil.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ocxhnqna.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2exsvgmwg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pundytol.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qdoinlzg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2innqlkyf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnryvff.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2twcbgdkp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2quzzaseb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dnheymff.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hdztzrfb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vuqhpsxb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lojxgqva.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vlfwqneg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwlgxwco.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ftswddua.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gclawnxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ivcfgomc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ozluafve.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uofzopet.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2klkynedo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2edfhtebc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2duxkhcxp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmladj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dzirsjke.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dnxekmot.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hxhbtrlm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gezsigvp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xaxrahis.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2meuiayrr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2corkkptt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ugoubylw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mswdifrb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqkyvqt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgkuypdi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2woccynsp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ztrdsqdt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnndpf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eujapfgg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wgzkscqe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kuenzzes.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yyolhbkz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xxcjpimh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iuxzlpln.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xnqeagul.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lebbnvql.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kwvsumpq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sksrovrk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dftncmrv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rllfncwq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2peglwuzu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbpuuice.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pjnhfxaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulcbwtdq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ebyinxox.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ambvcwcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2aencbcbp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nereiquv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ouyxuzrm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rifizwqi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2crhjiwax.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpvcoudo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2urtvohpp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ptlfjxuz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2isftaonr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgykkkfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kowxhxea.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2oeuzkiuw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ulsndmfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hpszjizu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eupuxlfi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2guvwmlex.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zlfoptng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2flyvichy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lmbkatxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jfggdjfh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vdytrgoc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mxudmdta.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2olgkhcnt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cjmmsumg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pflxrgii.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2urqnrjfa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kxwgxbtq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ijwsrdxo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jzdnjtto.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cgtvlezw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nkpbbpay.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qgoxxptb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hbljhted.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2scdpisfy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rwdpvljj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lmsyuzqd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2joexgshq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zgknisef.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pukcfgtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hybbsfpn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2owzmsndj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wahtizef.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2quiljyxm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wtkveqey.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dfenuweu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ldngukao.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lqhiijay.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qhzclmst.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ibjjmqke.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mzjxxtyu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kjxekxhd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvkpzz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dvfjabxf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvenptrr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpkgwdh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kdwfpdry.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgckwpy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwzopyc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ypduvexz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2flzqpoii.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ornwmjir.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cozssupr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2umvbolkk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bhpzfhwo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2anogpmow.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fgqruxsf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oiylkwpr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wnzxalye.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xwzyelif.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kdlkjfdv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mfewmlan.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ktjasbxs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xsmqfwrg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2townsszc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mfwtpgxs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ghhidgch.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uprrghje.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fxrklvlt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pzolexik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hypxnhky.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lbaigdgc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lccyeajz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ihyrwjix.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ruaqgkpz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2swsrieep.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjfbwgtn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kxqeuzzb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjbbnd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bccnqzyt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2skhaombo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2myndozlw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dusruvpf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhyshlg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uocwnfoe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yjywiynb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdxqyrd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2skuzsivp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2igjxdujk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uraefzuk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gckgyjmr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cqhpjxmi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cgwxqlad.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yksymigg.html


<!-- 参考信息 -->