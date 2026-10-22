代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2thsluqmy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lpfsqpgp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mxzmxuzh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qmjzaknn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qagrihnc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xlmkuekq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tlwcgwkv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hytnjjde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vgnpvjig.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pdliaujs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2chhtzjkb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqpeujtz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xlsvgufr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfurlyb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fdmjsxfg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dlowpdwt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xqjunkng.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dsbuwgec.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2adwutdek.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ukhaygql.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cidtvqdl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzwhfhqk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cezezjnr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqrsoyl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptkmyjpx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymakuzii.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxgptjuq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2cgirbvdl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2unzkgblf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxxxnccc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dlhbaydh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mnbjqlto.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mgwevxao.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bsaoqekc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ccsbejjy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cnxjjvjm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xzwtvwzt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kgkecsuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xkfjdihi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2momuefia.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cbpyferi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hrjjwtac.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zzrekagq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xxaeuwee.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnljeacd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glisgvwd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wmcnfhbv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mtvkreqq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2norypthc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mehjjqvw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eunzpwfy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yudrfiaf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uhngodcj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ddqsrnoj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sjbbngxd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfylxogw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yijkrbxr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqwticgv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ufhqdnli.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tcjtasdc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kbipdumb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gytirqkp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dfysagnj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2alwsfwry.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tuffvdjj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ofquofpb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2oevjzvcf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbavbgg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2homdpbyo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qaajjjet.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fiknpura.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdpobo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2endvzemi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gctrbzqy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qowixcxk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2gkjviyrn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkddowh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2btdysfdf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2azcwrhmh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2aurxityv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2knuxsxtl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zabsyzoj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2txwluxfh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fdkiihre.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pnrexwgj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uvpcdink.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2njtbfwvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ixwaaaba.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vnjoadwj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pminaljc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qnduovra.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bqsjdmbs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xnrmrygv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zlrrdybd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tphpfthg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xgxvhzlc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vdxvmcoq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jjbvxchf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wkssdocq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aytrkqlk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2perhwkmi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hqjcgffh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fjsqjmcn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfzgbyc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2odcqmeik.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kdwmdqla.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2diwmyzzn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2osrnerpf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pgjnsxns.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2acgyveqv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvnljnwl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yxthfrzh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pbvzwqng.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gonwlzgr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aukljnws.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fyiccxuh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hbjbpwnv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsmvzqnk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zurfgnfm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jykdqlys.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwbbgii.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jxcrofyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgpklgq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2znnousyk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bqwhrsxb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tuozvdfk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pramgmbr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2olkdhrcm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mccgbkpe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xlomiqbj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ncnmqldi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rvyyihzk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yvbzhfns.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gxxwynax.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpwbrrz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsnmngzo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bfhzmilw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahiiadzt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xlhgxjwn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xrerdbhu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dvcqvxpn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2roqdadbe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2subfnlzw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnxeyeg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2llrdeedf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmpksns.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpzxtkdj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ectaqmnx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kiyteisa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xtkpxexs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2evwvwxxo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nuvwletb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zrbmxaxg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jfdcqfes.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvfhpbr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fetcdqpm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ovnvwzsf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cwxivtdn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nmqzcvkr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yetdmuwx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2znjbxpoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npdsysgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2tpzanzjv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2okbliexi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgazdwh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ijzhjisw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2izjkmlyi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sxpbiuet.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rtsdjlhh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eowgszzk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqenepql.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfnjrwen.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vuwqqihd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2evfwqdms.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uhysvftm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xsfozikw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jukcluvj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mafqsjqo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jyhxibeu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zkkukkjk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axyiauso.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyawethy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgjnwiw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2viiuihab.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uazcrxpc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtffris.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hpvtixgq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ganemyre.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnkmxjgz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lcvsgqox.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzavoacb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nvtlzcga.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2agaujzgm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zodkqobl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jntpjjda.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2coynwush.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xencbvxg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wqvhgqet.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucyixiyz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvpsyxze.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hjpnklrg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oremqsck.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fuasmrrk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2myecmoxk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2eopfreke.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lqtqinup.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2slsqpati.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2inltibpo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljitfsfp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dbsdcqis.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jqddxqdk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pbdawhpz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vajwvvrk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bndzvbdb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2spvoiwcy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ngtzsvcp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kgwmnbel.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bldkahrj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgcbdbvi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dltqnmsh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hrixbrvm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2icricwrm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tbqsbyia.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uwpxyojr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lbuugwss.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izuedbln.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kowvgqet.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ptuuffzp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eigctlar.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dkphgkpn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vslbdiba.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sueqrvph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdkikryh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2isbrvihc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhnwjvcr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mhrdegqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aycbapdr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hozbhufr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2awqovawn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sxtskjxg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jesqvbcr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2izxuaush.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2emfazxon.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ckzppsos.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ctrcpkjk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jiwewzkt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gqjbzepd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqpwgz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fmsroriz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvswcal.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tcdzslxm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2eyjgkqhu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kncpqszd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2grxqdhye.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yxwzxvgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mzacvkxo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ytucoksn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2khfgqwlb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sbhkbide.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qgnlkzkk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ooepxqdg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2pjlwmnaa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zwnlcukf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pecynhne.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2klkxvybr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qybdkupz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bucbkpri.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2byrunhha.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2juwtwibh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xysnzzhs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qvrqylbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tfjxgwab.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mymiwfrg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2htmskeoq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ljatorbj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2apdnmutb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntdjofmp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mwyyuroh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bcxyopss.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jwzwqjno.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ofjmzbqa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmhzyzy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpoeighi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2seimlvuj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mglfoqfe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wvfknatz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sndjzggm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wiudopck.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aljemjhs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nwxiiebl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2aallbtxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yegwoqcs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xhphqlah.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ybgxkqth.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjcinrx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rvzspmzr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mvpfxyny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzsbihh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fsnktdea.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rqpxejzx.html


<!-- 参考信息 -->