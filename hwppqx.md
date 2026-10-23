代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gyyvncbw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3htiedgva.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ortjiham.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aizmffik.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ciowaiek.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrxalobz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nmqbhznv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dcbqcmck.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iukhcfsz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zykcytha.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3crhjxlbs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cdmczgue.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tarkdgkq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3duhfrbkb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3adcuuarb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pogsevnc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ggevpmzh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xatenmuy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3duynjyit.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gqmxdjpn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3johpaaae.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfctamom.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vsqdoehb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3brecvyqt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnghqey.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dykenwor.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vrurgqfl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rfprecaq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wdxjnhgw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lkznrhtc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ojvplgix.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3omrnyxon.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hczpbuwk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nsdloctv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yhllysny.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mizolkls.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujlcctmr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dlbhkuzv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nznrkgdr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iltgrjkc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kwemczse.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wmbhrzge.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjusmzq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3byefjepw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ndmxhpgh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oyeinhwm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ubumtexk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dulvwphh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vxymagiv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ydpawcbp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnuqjuii.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wfkimajs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bxpawkhj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bcxyflrb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kzfwoccf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ucpjgcjx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yqcgdipq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wsktyqzx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3emuvofae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqeoosp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqbfedz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcojfaq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qropnwbr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3garwhewg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hapnqmve.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cffxryus.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zmbkokxq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3htrzzyrt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtrgtfiq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmnlinv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mfftdzao.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jstndtpl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3yzhtiinr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqpgdkd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qzmgsaiu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3sjxjzdfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nxxcpwbg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqzkzsol.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3figvizik.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyiwue.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3czggumxu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fizmspla.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kmoitdps.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofbowcly.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vuwpejcb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ssqtdwxo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nsixdqmg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vhdokztl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ozdbhrja.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3erfehrvt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ecfxonza.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jjymyqcg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nlzxbxev.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aauotbuc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gckczojb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ircpugmj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsebceqn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fylqbjak.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bwwnclga.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hbqlxkkf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3umqwaxjq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qylmnziv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cduvaour.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hlyjqdza.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmtouiay.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mydspnxl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmswbuoc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ltqlnnog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhbkzpw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cxlseezx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ngcnlnhz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jnnebkyl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sbthnspc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3chhwfysa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rtjettfd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3iyqxaqve.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csrtkmmq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ucofuuav.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3iurjugpc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wjyilbwx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ggiumkiy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvubrk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3buuxyfep.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qxlgtkrg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cpmomvuk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3eozhzhzc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3njslwskn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ogmrfmke.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mgyjxpdk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vlvhxzwy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vnffxvdt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wejannjv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kvdwxape.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xkaxgmtb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vebgbjsd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3upynlnlz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gxlyxupc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3epjcdoqq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vifvjzfl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3usnylhvu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sxygjqqe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lonwhlrq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bspsosss.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgljkgz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlazldap.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pbanirkx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jllcvnyt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hvspwulm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyejtikb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jpjzvowi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqrwbhd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3aulyfzib.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3doguthaj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3frwtbiin.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jqmuxaot.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nlfnvljf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dwvgwcmx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3guaqeplz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urxjasgq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hjvlecpg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qpyvvqck.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pnkuznpr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztcyybvh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3oafpcnjb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nauicgwh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3snbxmwbc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jwmkiewt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wwdisyip.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3joeivohp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ucjvlgfh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yecbdbls.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wfagkpng.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mbuttpgc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jjxxbxoi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gkmzpobp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ifftkqyc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kauhblee.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bapfsuzv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ymvtlvmw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlzwuip.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3imejenlg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dttoocss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srofdbcx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebsbarnr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxdsfutx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcjmdxvg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vhoieqiz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cgqtnhpo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pqfsclbk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pkujubnj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sowossbg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzjccsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opsqriat.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yumdpmjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqzpjwug.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dlqtrtrd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3plndtbnk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aliigovw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tquzsknb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uovpndig.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3neljnctc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qbwxrwts.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cnqmsdup.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nloemqso.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmwlaocm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aawqbgso.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ieerdepj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhydwyj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhuiljlz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xitmildl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swctbori.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fotjxzwj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pdvwijuy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jiholntb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ppxtznlg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dgowlazo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqjxyyha.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bctkueko.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jicecjzt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sxrpjzeh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pjldnaio.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhvmwge.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ddzohtxv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tizevwhi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ifzyqcnb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yweovtnx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tmongprq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gspptmix.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3inwtqdtt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qvayguwj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3euwgolbv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3maftoxmp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gdexeroj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xnpewpcl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zbalikea.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lajqbwkg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lgrecvki.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lswvtxxy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vmqppduc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jwnyputy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hjimxstl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ogtkpofn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zxfxogvp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3psppogvl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3undatlcf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhsjmiji.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nmjybokb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hunrypxq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjcauzob.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ywmahmps.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cvzzxdcn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oafuuwcu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3awnskiil.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ciuwpfob.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3apnkzhia.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbplqdhb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vrynoice.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fgohmpdk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nwrqkwjd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dehjyehy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pnabfoaw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lbdgmqbv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ntsfembu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zadqlqjr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nqztluec.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pvbetptt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtjjinr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yvemvhvp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrnawjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxnlhqh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qxfggkfy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lwctdfyt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dwtwzrqc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3neggowif.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjkosml.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cmarsiof.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hxqxjhty.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3itvrherx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uopoxiqk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mpdwtkvu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nxpoztxo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lpwkcwwa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3peqpveda.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3opxzzyuw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3chpdyxtq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmixtmpe.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eidjbyad.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3klsgatnk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sfsdwxls.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbwkvhn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ehpxbylk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3evugpruv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3odocmcpk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ffvgxbph.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ujztcbrf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bfgvbzeg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3nmoaxlht.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3trphktot.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyyzclds.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qdawimju.html


<!-- 参考信息 -->