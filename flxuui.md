代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3agkjoewt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sryfddxc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gppmpfak.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rsdxnwpe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fuyeecfh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hfvkzcye.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cwodshvy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jbpskqjp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bcfgpoin.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zgndalnq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3opbksuvr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wttokiat.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ljupnmqt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3akqwjzur.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hvorbprz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wquzduvl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fhryfrgy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ahqkvvxp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3znpbffhs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gleincni.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hquekgcw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ovlkubua.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3svefkyxh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hwfvflbs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eaytshoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mivwfvzv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3siwnfhcd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbailzpp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpallxu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bxmblavj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlvybgmz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gfvrhmzc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3uwplftob.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3miawyenm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cqvytdkw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xkmjpual.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ouptyqyq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xasjedej.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bdwmahos.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ujqchxgw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xaqzbsgn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnrandpu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rpphpgeo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tyktcsac.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3abpiytci.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ssgontef.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pmqmzzcq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pshxzffg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nacuhbmq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pwzvnhbm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ksanfwzy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwebvvb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbbxfhxa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mcyompfl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pmndqkds.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yxdscxpk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxupygcr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzqnay.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ddhiarfg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hoqhhtoy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xahikjwt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bqspcwkb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pmmaeygs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcipexd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pzvjietv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uyfaprfl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3chxuudut.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pnernxvh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lfibixol.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zvhcecpq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kjvcevga.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3jxpsggdg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yhrxbdho.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kmgfzmli.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fgeytwrs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bbzfifyg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hoynxsgx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xyhterwl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cfbqenvw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3euqfkyzc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rvhqlylh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bjigcznn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cutwirch.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jxflbamp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mlyrolzq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wyglaggd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wetlvjrd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfpnfzbd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wptfoewh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pfzyapqq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gsgzuxaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hvapmlkw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dithwwws.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bljglynl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gbvchtct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kgqvpzxl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhlefs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3enmajqis.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3krmfqjta.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yrchmjab.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ahuwwevw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vsjpszns.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3upqvpimk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jnwvdyip.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tizvxgqb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufmnvjnw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmswhchz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3adtkzbcy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ppbjffug.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dvaswnbd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tmogbyrf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yfbmonti.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3msmnmvht.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nplownux.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xcrnnzhg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3bwhjervd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3smjtuisg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nlmzfczh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvawtib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oghchbvr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbtcnsk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eczinwwk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nicxqihv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yotgfzvj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tcgfyohq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sqlnnenl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bqilsran.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbkleqtn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ujwtrivo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ljbvtwnq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqpbsfm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vsxntmzg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhpufmmw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3krytkdlp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gltsussv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yrkfvucg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pxdvitbj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pgsrigcv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sewqejtf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rbfuruhj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvvqtjzo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3orujfkco.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sduugfmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3adqzcphd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3udxfhvmi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xipycupv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3roxnqrtx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ugcktqtl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xsrvhrpz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3frymxmhx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nxmsftef.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ocbkivot.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3onadtxkm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3znjcwnil.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnoqicoz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yyjdexca.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cuzfccxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bwmvvaza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kenkrrwm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3atsipijy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ownmwhtk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mexmevbx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gkhxlnwl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uwjnltga.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pqieeihy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qiumvwzs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyghyqre.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3unpccrul.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hryrekkh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lenhaufl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwejlek.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3swuupghs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgesmarr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hzkhrhuy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgktsiap.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ebtiurop.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3aozdmmuj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzjvbap.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wynvnvol.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fpfidcyy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3itynggqb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvnbsy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3targxjwi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3smstkvei.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sxckinev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jkcwavbw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3emuhsisj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sklwsuot.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzyfvdl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wrajzhut.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kjqfiwfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qwunhhpy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fvypioku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lnuvvjvb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nnximcac.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtbyodn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ebtofyha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qnwzbjbm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dcwsarnf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sefmbvsu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qhcfnski.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wleepiws.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3yptcnkck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zcrqbdfh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ujflhztm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smqspjaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsaavzo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pqbqwgwl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xiftcslw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iocvbtrx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kfeevbdd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jcyjqygj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lxatdxte.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lzzdfnzh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfkptfm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qoedvlsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmqmreoo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3smlspokh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dusxpbid.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tipduzse.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gtyyhwas.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3vkkkwwhc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3osqvkblw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gopwailg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nebauwkl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ympcgumz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fskkzaut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dihedzyu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymnfbuea.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iwgbsdxl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hbbmcyzj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wftbvady.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcjtcatp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3luerbnwz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vizouazg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dyetjqsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3phdqzbma.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3clhedgcv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bivtvbbo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cbyexbaa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kvjfxrpo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mcibuojk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqzxvhg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wpnnqoyf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3klwgllii.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3snzzgikc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3muqqfcrl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uwbimgrs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3aqaepjkn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rfvhjdvf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xyckavue.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iazvjdxx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vwqvxmnk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qvijaqwj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rvqiyrah.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ieicfotc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3uytcslpe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cmyxajyg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zjdmrbhv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yjielypo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kpyfndah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qzfwjcwn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bumeftxb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3opjidunk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ykuifeko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyqwrhpo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lqaeycia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqcolnuo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tspebrxb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3upszyuzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhyiydu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfxhjaix.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfmifzvj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bvvgajxp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zmbtdwrk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ksmhhxfg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ezhyyzmj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxjsezmg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tybyezlf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3foetcwhd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xlmntrey.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyofrqi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iivicums.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ttczzslu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3baakbtgr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pyxriuyh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqrufdys.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ultwcxwo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhjqozpe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ugiggmun.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rluidzin.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zjzvszea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bxkqmcpp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wowqskhy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iucadcyg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xxultngc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3klizblrg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hvdmirzv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bncldlne.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqbccnkh.html


<!-- 参考信息 -->