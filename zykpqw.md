代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qolkdinu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tdkhffcx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwvadpy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrnsmqog.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nemmqmyc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vigbuqgl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zakmwtsu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yczfgsgq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ussxvzjd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3otnngcaa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jkastkgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rlgbedoc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lyiohifc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rrywmxga.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3knuqrdtu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qsvhzxqd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3daypkbjj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fygtrsou.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lknrgggk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pncrmfpv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3axlbgsdo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eiuiacvk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ldhcipvc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iscibvbp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrejmlls.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3awyiqzzl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vxxzikhx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mbezkafp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qzhvmjjk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3khsusnrc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lvoysmrg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gunvsxsh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ebvuxzvb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3apgaqdjc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dpvfyznk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bqmjsviq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfzoxlih.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhwciqmu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3japmyyca.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fyvcloel.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rprekzsj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fcszjiaq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bsgwxdhi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pqaqupmt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lmqwtost.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qrkztgxb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzonhpbh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kdskxile.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwlmrf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yvfjisym.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3azzbyiii.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pxawadca.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hkpnhptm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3szxttwhk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3afyzkfft.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fqovkxpf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fentuicc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fasnezta.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ktqdgzof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3drddjncg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3krbkfwec.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dhvpkcyq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qvnfrptl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3epgkrmqn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3teleaqzr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jlurksoa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3znydshav.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bjsiodxp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3biuotgnk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dxfyzkub.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgwsfkno.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3geeyksux.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3awowjgcm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wotngvyf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktahqdag.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nomhebfm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sjiljfrp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wxbnwezh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lbxsjxpg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fjhzburp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cycuzbqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3upcjxnya.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjorhli.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vcfyuibk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbehwue.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fdkvrmrj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pcaltdpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3skqbzhfd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rhbpdvro.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cjqsfzwu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcdsmtmp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjftbhnc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zcenczog.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmgwugj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ieagcowz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3umgvqiya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gmmqedqp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwyempwi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uupzrqmq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyeokgcr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3crwvrkrh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbofotfh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tcuriowm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3grubjlfy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3khwjmjps.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3asfovyld.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lickjdgk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zfmxrugn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cnfbssmt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3brszzpqs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rcjavthx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3eoldsrjc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvejvuaj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tblzyjxo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jukssepn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jhvybyml.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3govpsgub.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ytjhipad.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gtspovmr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nwwbdzhq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nwlhwdfb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kqstwpze.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zwifmrwi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nizdbqsz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnpflqtk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ylpzjqbb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgevvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nxjjomrv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbgyvpgi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rnizqlrb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mbdoautq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3viingsrj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yjjkyebb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ursguxyv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pbglrlje.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wocrcvsf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jehauddi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3unmnkudy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tzkmgmcj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyrvmqkt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3moumlvlz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjvaxgcv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3merydayr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yngdyqsh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gjnlswxa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nlimkflw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yqwwqwkt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tzivwgrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3oguimkbk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nssfvfav.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxjppzcf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnlanuod.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bfxpebjk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ngpwgabm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3psztexbp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3usdkwfkq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rrgpnfzg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iotgthfr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tqhtjema.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xhowhxgp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zbhgdnsu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jxzqwvmz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3thwzksea.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ghhlzgxf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjfmxnrl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfvyvbu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xzcrfiho.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mzthlxpm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3goqfruts.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lutowvgp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsabptwt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lpuylhyc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dglnssca.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3khxghawo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3znftdfza.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ryymsxjm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gptkjoei.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ovfeeott.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrgoywzz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kxqhsgci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3brriiwgj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlehshk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lalmcpaa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ibthwuus.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qudizrwh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dvygshcn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qbwgotmo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jjeoupna.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mizbzpti.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xphibsre.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3odyzbkut.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3olerglic.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jiyyggko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ehbfvlwq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wrvualvf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3faplzbcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qiyypmas.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afhwcwaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3imgragxd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ugvamgqe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xeavmmfr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpugkmz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3utmzagox.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcziysay.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcmppder.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktngwrkt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hvopklsy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3npaowvgw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wldjxztl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zxewgreb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jpsyapzf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vkiszako.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvtsdqnv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3elrrccma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koqckboc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsqdxknb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vuwsemoy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zperpxwg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3juvxasne.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kuesxbti.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hhfdcprr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ofzxnhlm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rrdkwzoh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfhimzjg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zsclynsu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3resnffzt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3svsfzfwp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipfptvyn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ymylnplp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ufozfxqn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pobajapm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ouvclhnh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yryurjdi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xbhwoaab.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zgveapck.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yjamzlbk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xcpkllfl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sxgageky.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vusgqlwi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gnqkudyc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kqrrofau.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uwhcwbyc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nfndztkt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jlisuqwy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rwdmynej.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lsskamuc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dxetkndt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3exsnbhii.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ibgdxuyc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ewcilkhi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sbhayagc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fuuwxred.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dfqyfpcm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mdckjewt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pbmsixnz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhbthn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ktccwsrx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pisieirb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gccmxeza.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cdmanzhv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ikprtwiq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3prlwsbbc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3koqhwswj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjgecgyj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hzsbqphh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwtvredv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3koueqiof.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbnrgutr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fxidnyqf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jmvkhykd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ntkfysxn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vlscazvi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hwzkswix.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ejkykafe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eiorkoju.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sauwamqo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wbkrqfhr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3depbvamd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3koygaskh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qrbbhmbg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pljxghvu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xdwysohx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3feiawwlp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvlfeuf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3sxmajtle.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tnivlzlj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mqyozoxp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yphfexjx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhcuvzi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3shfhsszk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ilogneqg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bftdijqw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ialakyfe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tsmbluie.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzzezvc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mgilguof.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3humlkvxm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mpkqsuxh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ksroqxop.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lvlurhmu.html


<!-- 参考信息 -->