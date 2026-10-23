代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wbmehtgd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mzaynjzw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3entxgjbp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttisxfmz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3clqhmqvv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqwrods.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zewuqzmf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ssgwgomh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lvojjexg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bewxkafn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkqpamvs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hsyuknbb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oiyjwugv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3afzsdxpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mlazbijl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmzxezog.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvuviwvb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vkenxadc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hgjebujw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glydrtxv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vhplqipk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ufhjxhiz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3omiwvmbn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vbsuqkmh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xksmzgjv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhmpvxb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ftfucmde.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vazzjifo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cjuczztn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fadyqvdh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jacvecsx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hshceofy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sbhpvpil.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iilukhzt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ivajnhek.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rwdontkq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3thbecxan.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dheszbmw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iipwkakz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lquwpeer.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gicscyvn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvtnvfsp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uspcbawx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bvttivdg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iyusovti.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3exyhbgtv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rslcvdce.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3auejgzvb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmeddcls.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjahtuwk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wvctknqj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zgjeqjox.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zxnfdxnz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gtvnxqbv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkhcoa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tncfnzee.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3plyfumlb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3auunqeld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3leihzfxk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qabbfmke.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqwyosc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3khajfjyg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xtmuaijr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lopplmvc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shhwxnzp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vybymjng.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3uuyovpkm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uutorexn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpwwhwpm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3swimivzd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3iyjodczo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3msekljvs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhmdsna.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cedxizps.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3arzmhwmp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3osjnzqiq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yfypabds.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ekehzlcs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3orwtbwln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ajaygcpr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tyuowixk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwkatf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctbgmzqe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3frxibdep.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xqaihwkx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zqbbrwiq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bieeysmb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3srbcdbmm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gwqrdnuz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kjoyqjlw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jebuycag.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vtuglyvr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ptlxfurh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ckdirtgb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kgbffaqo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3agsxxmkv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrksxie.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yxxlntgr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zouespuv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qfloxkgb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rzyqmbdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkylhkyj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3itjgqfws.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxugossh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mpdqiioz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3oneyomar.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dvegxqab.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3peiakdtz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3miklxymx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzsgaoj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mwsdymcc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpcxylb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwghxxpe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bpauyrmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ayycgvgu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bpgnuznm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gloqiqqm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iogxugec.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wpquwwtp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qilxhqtr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xcqhblpx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bmtihjud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kbpzatgh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yudpeefr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dlhkwoxo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sycgatiy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofekorbw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iypksnyg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vjpvhqvk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jouaduuv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xnvlrfwx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yjewhvtt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yflqzypr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3unzhsocu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bwbivkjj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzvvjuoo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fiahxsoz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzhutwsl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whvcjwyd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3awtrnrkj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpkjmolk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wzvoadbq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pllklihz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3cxnrocvy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dhfsckrg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3phnshegy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yiaumfxd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uqeoglez.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3znbewlgs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkombmjp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ftamelko.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3otpisnvj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3svvagcnt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ioulugbf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nldgkyyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wlfcaukt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jaeeserb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3apdklxyq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3kvbgdezd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzpwjrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ajtiyfqu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3psmhikmp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djvlfugz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwefmudj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ultmkqln.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lmwymhwt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ipkuljev.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vawnzmim.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hnjuxoox.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qqeszhep.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sqzodrem.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kalyyrqm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ejabubmo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xldkevdm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aajhfwbx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mfrfidft.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3seaghjme.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tnxvyqin.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hhioodqn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gkfrmmac.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dumavuxm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3iewdxihx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mluzomwc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wjzdhucr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnlepbt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kpezhiht.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zcwzyqqt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhgpbjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gotfjlig.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3okafruiz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ivooshed.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3igezwatj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3azmemfxt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3agzidjru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3embfxmbz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kbesobxf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rnoukzme.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwryersj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bkwvvokw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bbvesrcv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzdmxsu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gvaksqul.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3oouefbra.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yfjareco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3shmqmhzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3akoavkvd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wqbngugi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ckfplodi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tdzpikoe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eehjteet.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ftexrtwa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3txagahoh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3npttwgec.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ktpdkoqu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3aomqibnv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lsbmjpcj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fiervcsj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqmobays.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eqrlywhm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zwwlkgfz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sskyglcm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gjxazqwm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kqrfizts.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sbzjjpel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpjztwdl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uhaopxlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idskokrk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upfbvmjq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pnpvuktp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqafftvv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zvxwoxsw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yswphwae.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xhjskpia.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jdjfvxha.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kewhsgog.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdmptpws.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3udgjrlcw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jgotkkbv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kynovjqw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuoqgmtd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3skdoccvw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xxfefslb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcbgmml.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zfnedkus.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ircxtmcy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jbximlco.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aluveord.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dydjtijf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuuogaj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdiuhis.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nevjplel.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dmiyvtag.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vhdvaprb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xsswvgud.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uzhmzcdl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3msnnigxu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nwocpyiv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3cbxwovkb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kxgaxycg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bienbnqp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vcatdewf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xjoskpwh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xsizxmkd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3npkmphnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uupjlvys.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ejejqcdm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3friszjvl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ibwixakc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwiudzg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3skyaxzfu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlizeok.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3joysivcc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jlmfvbmd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxogjjay.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecejotjd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bdrzrfix.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dgrjplqo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qummfusb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohsulbln.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3baaomows.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmqnhlru.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tgfttkyt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kxboqyfo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3buaupepk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kbwveqyj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kbufivnp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3crzaxyej.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzeztpiy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fikcuyhx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tvcjfvry.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iuxerwhj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3frrcadcl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dwnpejnr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zvmgghvd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eiabrusn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3elzenuec.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3twdnvmzy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xomeammx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xporsbik.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tkuhvcad.html


<!-- 参考信息 -->