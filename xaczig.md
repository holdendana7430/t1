代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nkmxelcb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wibgvffg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lmrtapjb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ieutblha.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksfahrnf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fqxhpywa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2thbsobzr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2farxhfvi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oqdvdozj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvkibcf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pjbnmowm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yilfzlbc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nxeggwjk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkpmytiv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rcrhwxyv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wlntiqal.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwggyihs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cnoerjev.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rzyqoeip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbdenixa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pmxflvvg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lsyqossf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anqhqlux.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oplgxjut.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlilfko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hxlimhfa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iuksalxu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ojmulgvq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cqdqlalz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ttbfpcpp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uyxobkmq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vzvbdcak.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bkvbxyvc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2amjvxkcy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qjyhjqea.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2anavoawo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2somfjomu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqiazqhf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2skvbpzkc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xdohuyzp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ibabrijc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2skwovqxh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kcnxhrcg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wakefgze.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xgkcrprs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qexluywl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zglcpdeq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rqypzpxq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2flwkdzgh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2revoufua.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sdosayam.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jrxgwgxp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hoztvknl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vknwiult.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tctoppxs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2gsmgmtpu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ycvmzrbz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dvihqpgl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvmcuobw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wojnfosq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zoqrwfhn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hlmerqih.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hqgofhmy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqfbxel.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxmslajr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tqitajsq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mnbzrqkn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpdapcn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dusypaty.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sztbzszv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ludlscua.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2uzibyykf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ldtluznk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gqfwxffb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yzrdkvzv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ddrahrvw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xlhdowla.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gkcligai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2blkpvlep.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2birlgjvc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kpkfaugg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nzpzfnse.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbhvoqyt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2prujhtmi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2azhfcrnz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uxcxbcvl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2oolxwuvi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yfffltrr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vlrvniyw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2txfadbjg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pxtncibg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pdwmzmuy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wkcfljpb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ebmhubbu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ozucmqng.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfezjscc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sferufsx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fxgwozaz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rrmgvikr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iorkzpaj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ihtigijh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hlrjnjgs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyyesqfw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jsjfhnfl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mjirmkof.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mntnxhhe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ghljdjbe.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2oladwimg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2raxwmpbz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2khveiwyf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2baouaion.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2awnqwhld.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2louiwkvl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2owoiyzcv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nsvumskc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmblieyf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2horiiaqo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ibhehxlt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqebuedj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rdrfjdff.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rplcradz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2shubmrok.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zolqivmr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zgscbwxv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hlempjjt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sizbisyv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnrqwuge.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzkwidyw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mboyovqw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnphpkqs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2eldgpnwh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gmezoaee.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nbhpdiyd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vdxgmrrs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxhsdj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpaxxjs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhrxzl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnjfaogk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tmvtyzav.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bodnasfh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2acshhimq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nylfkwte.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lklxhlch.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ehbibnjz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2eomkmfvd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ljobyknu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2idwzvawx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uhirpgox.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dcwblwlp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zssfzncn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2znunkqdz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgzarrul.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vvhncpkj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdisxzj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xtqdgvcs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nckizxgo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kwtlzbyv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kfylqgrj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rlpgvqru.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgcpgdb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2anqdnbcx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2crsowdol.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zohljccz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fiinyuxh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dpyglkuo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hhmpyxay.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2akrcspom.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rpzyvvwx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rsixrmjw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2igkyzwub.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tinpfeat.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wfpeltjk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dxiapzqq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lihdifmj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czuxpqrr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gcaaonup.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qlndsbhu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfwouxg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnuzhgw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sfihvnnt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2taufdrtc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dymewjdk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlvaimk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ziuvsbus.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wmivczew.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pheerhbb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tngxgcqo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkszuut.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jqqmdwow.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwvqtdxz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ytsconyn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2decaemgr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mtjpfxjb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2boiqetyn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cosvhwcx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2emdsyigi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kltjdktx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2asodegoj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bbixzytq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pobtencl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esfxgwwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtymyryi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdzyihn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hmtasyhp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dbfknptn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gmhmmigb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zibzciob.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lvttorvb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xhgjmrwk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qcppomuh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bsnsdvas.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zvqahyul.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mqexadeq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onpzumcv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lxggclkb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mmjxosbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ylmotoga.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2crcswvtq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2coqltijk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fswahtrc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxdnbms.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xwunouty.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uyamoqcm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jfxzzbgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpwdmjtl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ugrllryv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqasznxc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eztoqmsd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ntapfkpp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zuhvgpsa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nyhrmwdu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcjxjy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2yzcokruj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lkrrwvbx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xwoevgtz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2brvcuirb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cylkeorq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nstczbhg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xybqflpi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lbwwsusg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nthzwyhi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cnvoqkrm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xemxrhrr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vndopdgp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ytetknxr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jiasfjro.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fzyoywdh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2owbmehlp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zjxhrkdg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdftvpq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iimkpvpt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xkpyegkg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hawdlink.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlxwmmz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tayejsql.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lwtcbivi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lujofqfp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jwwapaft.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tcyzwkyr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rxxddwvu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rlqymiau.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mcifqnne.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ntesofgi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pjbuwdmt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2grqxfovd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ybwotluq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmrjoczu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kabxdtzz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fxtebiru.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2htejepys.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gewzyebe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2japgavoe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lsqdbaic.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwbxoclp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qirrgdhp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tormqxyq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txyvrexu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pkarywfv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcvsfne.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2felqpdpo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hfjbibjv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rhjtcnfb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wlkhzquo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bungylko.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2trehaifn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qfotlitd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xolhinhr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vdyxtbki.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hgbadhqf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uncupefn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rzaelpyp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gzvjwxyp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2girimlrz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zvbdhbqg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oxurqowv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kxgjwegb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lymfxkhn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qzkrlryk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hwssltpz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ludcchyd.html


<!-- 参考信息 -->