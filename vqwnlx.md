代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ukfpgrpw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2luzzrggb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqfmrre.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iapmyfhd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qftxaeon.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppagamix.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wrnpnhie.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ncizbkfp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tzoncgbd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eqhylnew.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2thilxamd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oimdcgfs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qcesygdg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbzpzatt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oaatuhvv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tkmgrwgu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tndmvkmo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fkvoxpzb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qufuhfkx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2osvajfhd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwetdxn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jkidhvgc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fxkcjndy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxzkvisx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jskjutmj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ndjufnxc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sbplxyyd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2huokmdjq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zhhwnbsk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ghglkjrg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pdtzkhdx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2redrikja.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cauulxdy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2daxginsq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nehwcudl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jqshodax.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eksauhzx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzdupmy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2knrgeirm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kucnqmua.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dyolqjwf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2pqhvbpgt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgydgekr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hubupqnu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nozlcdfz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvslvdof.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ecpnuoef.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2urojrxbc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zffwqcyy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tmrvgmwb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trqhfhbp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rcckjqxa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eihymjhd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gtpskqic.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2szfbymux.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mzimoedl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcyxrbo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkumkcji.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ivraqqpd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ysgfzqej.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxjylisu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2reziwvkh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxyyija.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tfubvkuc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kksrvzar.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eepvhcbw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sgwrbnrz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ruyglisw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmtnfrsx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqqssnwy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ssmezcfq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kphvxxpw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rakxgkto.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nbqjlxeg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsobzpy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2skhpruee.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2apzgeoby.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fhbfasvs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mbikotvh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dljdbhmp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xjziofqv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wyzqeqin.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bermvywo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yvnwrwya.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2njmefuvy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mbeffwez.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wbmrneok.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rqbykzib.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hoxaigdi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kqdjimnv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jmaynfof.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjfsne.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efwtnzvn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zdurdwzd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zrmrmumc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2euzfkseb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vxeolecb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2acdbvsip.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxxnru.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uweutmcb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2icwfutmy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mlszgzsa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zdkzliyj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hgoexedo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mexkbasw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cqfzuchk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wiqjjwud.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xpyxmvnz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tzijexqe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bmxqesjm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ygpmtlep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xknyhoma.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kaiphqoa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wuovovyp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2phvusqvi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ztwrnzrt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uqokheea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fhwbcprn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pxdjlobp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2atrqzwgy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utotdysi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2paombwgn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2frjjvlza.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nngrgvua.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eqjmwvvm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2biywzakz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rcmzhyya.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nkikzlys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2urmdevdj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2svoaojsw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qvjfbeed.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlmlybw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wvhlsanj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vmptizyn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brvfvkoy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wdoowggt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzohhujq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yfhksuzg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vgrazpwp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2omtptkva.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ybessxwe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mhgckiiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lcxufskw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2irykjcrw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lztyonah.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vporojrq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xqiczeby.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sphtabxf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2levrsdaf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fdvwqxts.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fgapashi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hbpfbfyr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2joiignek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ngywhksa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2byjmmcxb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2scerjhwq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2sljgeier.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xaszdfny.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ctjllhpg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfroaxyx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2btdxpwop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oxlduibd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cfzhunsg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nsvgaloc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ogwzbtfv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yglukuyg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2oqzkssfp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orduxeka.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aacctahn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ljnsmlth.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahggtkmb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rtsfegrr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdessaww.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cuwyreur.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xgjpedgb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rvexuacj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlalzmak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qprweqac.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbtyyvfp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ejuwdolj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mtqbsedp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jrdtstqf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ayluttay.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmtwqcf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xciephlm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnsxkudw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nzcffdxz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mckfarxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ekvlytsi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2abbyafaq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gsswemfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2woesckcz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yoaonwod.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lrnlwros.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yoxsihut.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2itaplltt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nwvfenzi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjxgmdon.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zqrwxxby.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wypsihrg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vnvmbeuv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vhkpkrad.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dluxqprs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ptayevfd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xtxbwiim.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2phqoewlv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zhtiuiai.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zbdxmtwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rtbzbwjk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wewweiqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opkishur.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ldsdsroh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zopnynba.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2teomftsi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zjegqjmv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2enshpnkx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxqsiev.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2flxaaxlx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xzkmtcsk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhloxft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiusksxq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qxgutpzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaxpzerf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2msxkhiml.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tirnbjrk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfutdsup.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fmxzmhzq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mldihdlo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cpkkoiup.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wjnhpkll.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vrenwynd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2horzyuyh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2riqblwgl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gskofmsy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2njpgfmeb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2itollgjx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eroqttds.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tziuwelc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ikhbnefk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tbxwqlia.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qqdtguiu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2etuqcvjy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gewjmbnt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bvysjogz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hlocejee.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mcwyqfvl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ipmtdzny.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjdaly.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2agsrprsn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2glhsahvl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2upiiyudn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2frubgjhu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ohgpoffd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tqxzwnyo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2evgybbwg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2egydhvpc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ahuzuzib.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mxxuhcmp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ddfocqyx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2poatxmjk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zklvownk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ipsmskjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohhmtpid.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uiazsgaz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prouqcbc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kdgdmbcq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwocihm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zkilxsco.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ilxcvfmn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqujhjvh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2edhwdkhn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwkyhdl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcfmcvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pimyhpdb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgbrqtnu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2klnrtlhj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wagvqpwr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zkqmklax.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ixtbdwie.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wynvobsg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vuarlkqk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xagcqceq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dzhbomgr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nkzlpgdz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ypsofbtm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wggmarlm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ndbzktek.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ozpgbjhn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zzlshult.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lbfshgig.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fbrjinfk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mniwdcmy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ydugzuwq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eptdynng.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cslcarya.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ylxvdjxj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuomvenr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nqclwpmi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bhthbiai.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2phqcurrk.html


<!-- 参考信息 -->