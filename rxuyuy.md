代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rwqcmpuj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vnvwdrbu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2utbkwnyo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qnzwqyhy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rtqtvdzd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bdzcggfk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pdmjyzep.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lmtzssch.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ldmncgqc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhtbklm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rkrdtxhw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oagneekf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gsmuilyx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2oroysihe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwpoyeqd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2oaussvsz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fljrsque.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtlbhnxp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tmdctrgz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bzftsdlq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bwjmizjz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zvwvpjhy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lbtqcaut.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2fwzgsueo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vqbuzskf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cqmlyhqk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ultdxchz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcclas.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wjyzxogy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hgifmwiu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2usohlgve.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wlqyyxht.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2igjjnfvy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oqwewuia.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bxjapjsj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ouzjjloj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oilaobdw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2coffslue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gbnkbkzv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wrmrjevy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anmheqty.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lbjqkded.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fooqhnlc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rhkhxikk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pdnzeqfs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bygwugic.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2plvmifrk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dhsuqkem.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hcxsgexm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qudydekr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2akdqoioz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjsyirjd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xihiwirp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qpqqhezj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2crrevaxs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mewbdjsx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2plvhytxe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ndovhwgx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ciooevbx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ytmspzbv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xpawohzh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jcvnezam.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tcttsrkv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ajcdmtpx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvkfgcb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywahhvep.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jextlydi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrbvkm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2psvozzzd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cvsmnrkh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rfdpqzya.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2htdkmmzw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2axgdvvqf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eeychcgq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2szamhemw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jdoxtlzj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2otnzsdet.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2znojpvcr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xxalfmyo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2itkevigz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nszkyaqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yqrmmrjl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkvqzgjx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2thbhjewp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tpcajnts.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cgpguhbi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vsbcwujp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jufzckri.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hltfzwpt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcmqpixu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptzcycvu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ifizsmqd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qxydmurn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2moozijfh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2peiukrlg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qnxzdjoe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yxpnqjsw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdljiak.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jfftdihj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwqllvk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msmwzvnm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjnikum.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fzpeujzy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lfjxqqmz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbgvarlb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2caisvqud.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ronqfifa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fbdgqqdg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gtykmcod.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2aqtlevjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bciynevn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gvkgjids.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ergikwam.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wpcsbtcc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yeulhtnm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbqsqag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lkgguify.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kpytmwlk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmixfcb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkttaege.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mwrwzmul.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tagyvybw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnoudehd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hqskbrsw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktdgjgin.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tleluenb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lmqxyvqz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hzyvhiyy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fcizbvnj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2shpjyxfg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfxasoib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvdyetiy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdhzlss.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wzijrbpc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kdagbbzd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dncfoicm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2acntsqeu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wnvpctkk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pneqnuje.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwdjgweg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qceptusj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tjghmono.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2sddbsqrx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oxveoihb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxylmdhy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oonwxuwf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cthdfdgj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xmpwtkpg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iepcreik.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cqvqaipv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fasgnbjv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bhalgzkm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hldwjilm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqjgwsij.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lbnssigs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aeiapqjo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eakszsqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2uejctcuh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2twmcxomv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cjinscia.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kquvmrkx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rsmgbseq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fwlsvxfk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttklxcdh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cnlqxiou.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wnjbeztb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqizlpl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blcmcxep.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ualnjtkl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2quyjwnyv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tleawufa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gwfspmhf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cumwmhjl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wwdqucjv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vrjamnzl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tjvwczym.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2raajvsfd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2keeuamok.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhrofo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcudvgtt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yjqzmday.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jghkxkuh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwziqfuh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gbhevxha.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pskrimat.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2inmyzxqh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rchbhkwq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2szajllna.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zjpaqyku.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pwcluqou.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ckgwtoyd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2thmbltmf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ehalwcos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tvrfehev.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hyrnnhhv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gsosgaog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ugmikjnh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ssyfiara.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rbieilwo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cagcwvnb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kobdweia.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xgwlddok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yukwynbm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2asienaym.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2anejafva.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fsihkxug.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xtvfaltt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tdvxiohb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2txnjiqsc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dopgcvww.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qgawbhts.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kmvddscb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhpvkm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2taxtsnsb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2milxxyba.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhzzosm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tivpbtqo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcrumtex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cyelwtzp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ajjriobd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nkefvxba.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ddiipjnn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sfgkcfss.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lossbysv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2llocurjg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpzcsagu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2netcveql.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2insynrya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tarugsic.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sbdufnwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjxpznsx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tzdedejb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2njkzlciw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nkylayir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ugucforq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nogsxeol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2emjetqsc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zcpcqlqb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fgihwigy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wnbeiucy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pfvpfvms.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2quehnwid.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tcggrhab.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuuvemxe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2djbvpfdh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkvozkq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2botrqror.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dwnfqaje.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2srbujmlz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2specdglk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sotccsnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zqrzsulk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjzmhea.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2euskbtqy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2axxzdprz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eydyfpln.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2aqydgxrn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kswbrdrh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hacxqvpm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hkkkijsn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pzosudcd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2foeagbha.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ihnjulhk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yotladin.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ccyotxfw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qxdsvpea.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oiqqzvsl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2khubmygy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsddfmis.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gztjkorm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xpasfagc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cfnqgbfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dgzwwfkt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pptxhxzg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgpbwkvv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ivcrwymk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xflzdkwa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2susbyofd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2stpuzfza.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wimmjdfw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bijjghuh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bgbdnkqv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bymscknp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2shmczzws.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kwjptmpj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yflvekfw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lrzzvpxh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2llzxjvwy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2odnmlivk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ovntkdry.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zeqrviju.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kybzvjou.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2khjgjtcy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2odmhgqns.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2goujphvv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sotviwqj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2canlyamg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ymnfqbfi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ywcxaykr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ieugthws.html


<!-- 参考信息 -->