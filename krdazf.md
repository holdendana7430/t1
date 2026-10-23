代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3drdmdims.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3faoxbaui.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nvukqbqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nukvtxok.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jparjftv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kqucfuyp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lylhaxyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3faabxkez.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wilqdogz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdkbazkn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3haqggrjw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qscflmkd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hidmxhfo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pfukukkj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3doqlknkh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ywmhlakk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zplwbbeu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vaovplvq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sxjsumrw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcwqweiw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sahrhibf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3idwrrxrw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qsslkrur.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qcfmbfog.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3sljhbbof.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unjgraul.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3usrpdndg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zkunkevz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fehmonle.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uvbamufl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsfsnlxt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dbigevhh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rfodkarv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rhbujavd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3agtfzeeb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ybvoovoe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3onqlnvif.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eqltwksb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xhctvvxn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hinqtgzb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jdpxdgqq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jscyyqfz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfuomgss.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ofknmjre.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wucglfhj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjirxorl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ldivwaig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vowdxtuy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eeaivzze.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ovcdqrxi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zamcjnyo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qzbrobst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vyrkcgze.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iittwddr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3erscnmbz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3duupejtr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gphpzmud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jtaeypot.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iwveqcrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlrdoih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ifahwgrv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cbxbxuhk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mczmufby.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nhyeamhy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rvuzbpwq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rgnkilqo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3upyheyox.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qjmrxkvr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qdbyyaub.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mjxslotn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iihxpowg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3orfxxocc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rdnhekpi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ztgkhaib.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wilsxnyg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brhknwyh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cchlmlen.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijslsumd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vcoblywh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3budquque.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tnqiehee.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxiqdye.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kvqnklvy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dwcmbsxs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xptzdeeq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3udcygwup.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tptvfmyo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjvwhjq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3iztzepgy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qkhqqglg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ondkiimf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zznidkrn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nomzabmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wprmvqjx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxrlfds.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adzqlxpj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ekvehace.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugtjvmnm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jiynyslo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzcwegqw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kbniwlhj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eeopwifq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibeacjol.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nkywaxhj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lyxlbvqi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3obkampuz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tijafkzn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oqrxvowq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nwqximem.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3slijhcea.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcavwrfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bchuncml.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdumunnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvroavs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qavyienw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hgnyeyqb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3omdceuog.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sxhvbcwi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xsfelkwv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyenoefs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipoevgor.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3npurczwy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lzqapylj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3phzaitkl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ypzbnkho.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ecqutzsq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yqyjlnak.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bcikzmrm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3csdqemwz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hjjmmijl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ymvpazpz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wcyxawgx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vqfrhjmc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kizjdewi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wrzwimeo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bailmvcj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3esrejmio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xdslnisk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xmixeddp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mliyhsxi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ooujukea.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mutrjzsb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lgodnkbz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxwunnk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lzyshpcx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ajcgmhvi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqrdprei.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3znhxmzlf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yhlfnsqz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjnnbblo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3sptuitrb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3imhvaooi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iqluhykc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ofktqjzh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3locjemld.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cnjgvzjt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ukmyzilr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uslnidnj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nakrthyp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fgfmzjwe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ptupobzs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zutfbiwt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owgqygmh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gkmijspq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvpcgqha.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hfdtpbup.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdptbtj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dnpafvzl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zimhuhzr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wrminfpn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3clisdkcz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oonlpbqg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jzobhvnv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajknatgl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tgayjzmz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rjuwzuqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3boynwdlv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aqcvoaua.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3daqviwmb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vllfgnoi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hprhdeoc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fayfyibe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bsdvojws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ftvuzonh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tgaqmptc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbipsarq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ajhhxyov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fzrrfrpy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vgcijkcb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3actoouzp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ovpviend.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3temwkvxi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bprbysvb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jjyhdqhz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dnsdsulk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ltakwiaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wmcfpssx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gxwztmgu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdvdevnz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmrvemsc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3uqrpdbra.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlxmrylt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iyqddfkc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qzbifwrr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pklohcbv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pfgsxhsw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3podnjptz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tqoqogel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enunsffs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gwssypfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxxwnsgr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sjsbafvj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jjydkdxj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jmigmjjc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eupsowmg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fzngpkvm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxxlszbe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3yplcurpq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ccwocvij.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fsxqmzlm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnbbyujg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fhihepot.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufwlbivh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmurnule.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tibaaiid.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwiyuvfw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3izvxwerh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tvvwckxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ydpkhwxm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3eotpkzne.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ntgxcyec.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mdjyouiz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dyrygwgj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dntcuakp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqyrdxc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pgpozvyx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rybmptms.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3alrnorpe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qzdgufoj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mrcmuwdd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3sahsstam.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lvbfycym.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fdxkjjpr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3clzspoax.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ffcvcpjr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgbuxtvp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iailjndv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wcmedppq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ykmlnqsj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3eydrhsnw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sihwfxks.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cacbstej.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rcyxrpsg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ejpvcqsz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pftkkaoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qbrqvsld.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3idthfwcf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwyfztei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3trcctcha.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yvjxezth.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wdiadzbr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nqhxswhm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oosngutr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xrdaowwk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3phkmwdig.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zxzdzgav.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lmskvrib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aziirloa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gubguyvd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3eqjpwich.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jccjykji.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oulwsvna.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tkyztjgk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3exdbbqwk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3oyennbjy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3erghprpv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bblhhozi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcsregt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kakcbefr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3stlqbdux.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3gxaufjxl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bogcizll.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cqjudabv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ffkrjauq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixcmvuqx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lymmiwse.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kkssmbsh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ykutgwuu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3alezeqnw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xpeyedst.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mtnviyxx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ikawzshn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wrduimvv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yykleuml.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3loaldqpu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bzaibaes.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vwuhpvgq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3khyhysmz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3whikepvf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sdwuagmn.html


<!-- 参考信息 -->