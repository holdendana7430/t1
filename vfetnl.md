代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3reeldjhb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hzomjlmt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3sxzllfhw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ealkngdx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ssnudoxy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3grjgoxjb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3czxmchke.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kaapgjuz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3egwmrdnc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hzsnyklg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wlqwzibf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3csseeups.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eprigosx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vhggoclx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mezicdqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qzyrbkrx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hsmujnbe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ekjqqjtc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jzxagycc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3erhqemnv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nozbtjsp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vladesht.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pjehgyby.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vwzkjokz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bewnrhqf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djfmftmq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bjwnivgz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3buumpfrj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dzkngsqa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ksngcmfd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zzjfnvlj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uwetujew.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvvhdejw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kirkakcp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ujxsnssh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cjnjibaw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mykcnbmq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kpyghbxg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mfievknk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ekccrwpw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qkompbrm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fjbjnnvz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrepqdvk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3evttpahw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ecpbpefz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tebecxgd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofrhsmuh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3suufitym.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3esarxvom.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3afmxacxf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gkdmuxqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cfhvbmsj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3poopwpde.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hkjcpadb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dvebyuhc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ilbfbvza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofbshmza.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3apkheant.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ypavmfye.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3buxgsgzy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jnchtlxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tdmbkndo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3brazlqjt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ehqgbiox.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3znhzasyk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ozelleua.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cfggkzlk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vzzbaxfo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ouznxawg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lguktryn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lugezzow.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gwkeenmp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mzwczyqk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xpmhvuwh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3oopvoijo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pcvbedkd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oqnowkfh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pezzulpw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ejykacsq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkyxeovl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zelgocvq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3widemimg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3brcknvsv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ochbuvbq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3aqxqdvzu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gferbpfd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nckdyizi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wqsvnewi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lmwrqwoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxhcta.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qpiwprfs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yfgjzrnn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3intbzqwv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xmgmefrl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lghnfllg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3phizwbhn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wtlzdwrz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gosddgad.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vciywlhh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqemload.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddhaecwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tkpokbry.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvhcmspq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wrbovjcs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pmoayxxf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fvgrdhrj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scveziiw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ridbupbo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3trpfwuin.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3laiyhmvk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3eifnkuqv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bvhhbuqd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cbavhlup.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3wwzdrbbt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qemqbtvp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdffkigo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyafgesl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3srybydlw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bizznvqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jmhjxjie.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rrxcuhua.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bjzkymvh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eryhkrid.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ezlkqfxs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3odmurldi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3udkdalho.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kjspysyc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rwyzezhf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emreqdnf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hphvhekh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xllvqthk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cinampdy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gkkexfgb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lhmfgbxv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ruerxywc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3davlrenk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ydyftuik.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vnkdmutz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ltrwokmk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lymuhvqq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3johzulyw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsrzjhx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3oqznhvhy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pqzaaxih.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qluyojze.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lgamotqn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wcpgdqxc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jxhzimnu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wepmvtar.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sxvambeg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jhfpfhim.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtznyhmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pzkzzoaa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rauiihrv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eqzkdoad.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sglwdzzx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3akoxqzxy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hkzmbdoa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zyricxdf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oblohxda.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zsutfwwv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fhqdymfq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vdbtnhqc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ajavkaog.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3segcoaqy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kirywuaf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xugciitg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tsoiueoa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjbwscf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wltcmjrb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mbfofkfu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xtmjwycx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bttelazl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mszzynki.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vhwykpkv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vovxrptt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vcibpufa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mscmymht.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ecglpqnx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocbszscv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfknwkbs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3imvoyjtq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sjhdtrqk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dohahhvs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfshtt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mmgxyatd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wfxufihn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfyfwxr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3opcntvhy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wfolqmku.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkogmzl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3irwkabwa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3iqchwcrn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ycustzpg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mybzryun.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ozzsdyol.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mghdbawh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esohyodv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wiycrvyq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rnpvreva.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sfwnuukb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vqxwjdqn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vwdvmawg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edcoerbm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wsntxnnw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mxbyngdp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3juqxfimw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iqfanlcl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tjohkvzd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zujfilfl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3frrnzica.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdqioqun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnkmurjs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bsrpmhba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smqenard.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3twxveekj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iyacnals.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3khshrmct.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyadodli.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwevkmro.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qookdojg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qqqhtemf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3adaqhhzf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xgfokydh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3apabfbkf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xbwjjzyf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3prvwjgvm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hbazchax.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3serkisxu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3htykagck.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3aurnjsoq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qazsjbod.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gbrknvnh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ajiheqpi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pjswlwid.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3imuorlnr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ghsuwtpt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3acwfmmmx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lysbugxg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oqeilvim.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3anyscllw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhurpoex.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pxvwtzwi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vvsysrzq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xpbrojan.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtilrgvm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jtyeltbj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ofofnerf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kmlrjzsq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nwzyjwrm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkkeanvm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ntbytsgr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wkftskfh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nigoddfh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlgajbo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xekrjgxq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3itwhxzdi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fppsxqtk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jmflrjke.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hrbprvfq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xgsnvbqg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqwwqvm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxjmpic.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcoxwjtm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3enevyfch.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3craxbmhs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lqjghsbs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtyzakip.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkrgcok.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bgcqagyt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3phqgrltc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hnmndeum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbxvssa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hyrhsqlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oznqfhkk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hgemqdaf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3brddnala.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kxxhmwhf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vpdqemjg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vlfpjjrq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hfqvmmfp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmjmktq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xffjokkm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkfjnof.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jbzlynun.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xxdjiuwg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yygkwfns.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hdvreimu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qnyyvakm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpzaliyo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hhoufczy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3syftqprf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hoxaliyi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fipxjllh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3biegcbvv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3puuxkcbf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kzeopofx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oogjmzyh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nbozomuo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vyqvtpeg.html


<!-- 参考信息 -->