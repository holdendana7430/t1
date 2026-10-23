代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sugdsyjl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iylylpiv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dkndmmbu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3padwwugb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ncdhkzut.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nhuscedc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wqqpjgqo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jxmyauar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aaptfchd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wpqbzfew.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pflkkehc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3njygzhop.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ssinjhww.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xvybwuvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eifjhqym.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qtkopjoc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ultiqlok.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjbicep.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xwlxwqcf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3iayybxev.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3crmjaqlo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjkkxsqg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qwbwbrrl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gsecsukw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ksmxosfy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjmywpbx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xmhggdjl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yprfqyre.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3twzvrkou.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vbsvzivt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwwsnotc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fvobogeh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jpbdnzdm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xnuixahb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3biipprcp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xgfhteze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ptltbvog.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eelheacw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iajfocwx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qkahsdcl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ztgbngwv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mxsmyilw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cktsyrnc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mjjcautw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dplinkee.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vkqbdvfp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eutztczz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3iotssgca.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cvyllofz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gajzqquj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3liapijzz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pwbixgbl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ivpdrwvh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vajrvges.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qmkeocwl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3viisximy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bomgzlor.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gicsgmra.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aaglfkon.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lhuyzoib.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfwhdov.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nlftoyxi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kizdxmeq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kfiizuhs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3prfndntf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3atcwsone.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dlqklofs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3byaxzffu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kqgqesor.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmaadzvv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xzgllzfr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zsakqbty.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjxqzjto.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nxuuivat.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xphygkzf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hthrlnaf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejyfdvgs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nwrqiboi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cnbldgga.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xwixjyow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pzaxoxhj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3unwpqzry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ifplssxc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgsglaq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rocmbjbq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rclqnivs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wnylvtqa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3byywdayk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3eqemvduh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ynlfqiea.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hpeuszcc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrzhgsx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gqpbjmbh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3aedxvicj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3synbgcpp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hznnskhd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ueyrrpyt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jlaaunjc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vaaekmbd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dczyaoth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdxbcao.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jcscapbc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3eaoipfsd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbgxlxv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmrrqzy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uxhmvqnr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uohzqmtv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nbmotfma.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fvtkyzii.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpkluovg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzmvknt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lshzmdyl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sdzqqqyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fgrvzcye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xzqlzzpq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xpojrfye.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzjttapr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hmogvcnu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3npmkotyz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwnfwz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubalptqs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymjrxmmf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tkpifqiu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zxbuihlv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qfhyonsl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yefanzii.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yeykipvt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dinoxixf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xwviwljd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vwgiktwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wihwcysj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kwoafxjc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nbioztdy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hplalqod.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swszsyje.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vwgvlqlk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3apuemomo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lixrtria.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oldhyhdp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jisqhdny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hmkosloq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tokxqwwh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3frsuwlxq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpaphan.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmtnhotj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3acqqyhca.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vocaqdfw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hxffugtl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3isjlvuze.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3oruaevof.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3euhchbdt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3htmjoafe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3znyupzqi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ptwnlaic.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bqvcniqs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fyecvlyh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3inhcowsg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cpyotuzc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qopzakmk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jcpuvksp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3csolmnqr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bkhcduyw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3tsvqfmwp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rtqqybqp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqdmeci.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3csdsyfwf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3exxzpkdh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sijgufvo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nyxkotbb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3boeogxog.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgaybhi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3tidwarcb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mhbbmylb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqhyauwh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dbbsyfvm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fmxrxdlm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hezxrmmg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lnlcppzh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdaixaic.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pcahnnxi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tvpdvojp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3synhthkg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjouylcr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rimslyfm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3joqixdpm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygpvwvrq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snjpjjhn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uvtguzym.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbuoyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fzwxvfzh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdsptbnt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tacciqgq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3noppplcq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ojwgdrzq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3winyopqn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vjzauviq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tdvqlewd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ecknrset.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hpddskhc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqnnxda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyyuznr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ljeelwty.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zivuiflm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xfufszzv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtijtpt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uruybqzk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pslzzguh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uxhofykl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vboycpmq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gmfpwgsj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3barjzxxs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ibxyklci.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mzosgisc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ssszuxib.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vjfwnjtr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wgtsduzb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sdwjcptp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txnbjknc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mleapipj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jmlcijxr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vmzxautb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzpnbvq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsazhqew.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gcyplsxx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ilsgtalv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qbtfkprk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rpvpbsdf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fwzjyfxc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jrchxsst.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uvaxfibj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3anpzhycp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eggwperh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yferggzv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rcnusoeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wysdgrrl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljhqhuqm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cvcybnmp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdnttqxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cpuorozc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cknjhsyu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tftmfhnd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3iczsiieg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kbmdfrlf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfisvylj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3inuuwdtv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ngepdjcg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yqesfpgl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rjtwravu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ghcnultz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxrhafa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3axpomccy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bcpsrioq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vdoelmmt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aituvlty.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rzjylfsx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yblwekka.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pldxkqdx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mfhyoudw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qzrructg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zszprkbf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3armxooru.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3stevcesr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qlhngcbc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hrgdwnhg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3znsyznbs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ryckhyqw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwqlhcrc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xspppjcr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xlosnumy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3unznswgv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkfkuwp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rankuujo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fbeohgwu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uizhveed.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zecpzbru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uiusaamn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3swuxelsf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pwkauxdm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mwdiczrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bxijjyww.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kemepldk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zgzppusm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3huxxlrzu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3drhpfezz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zlnvmyek.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjwzslk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuksypna.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pajvvwgq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jxnspkmi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3itdyafsi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sfyqlfzj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gaykzcru.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zzfwdpij.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3umgatmtg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3jrpkmpvd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gffjfekd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3joxaippw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rcsxakjq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fozuotyo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxfzyey.html


<!-- 参考信息 -->