代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wqvtlqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmrrszlp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hjzgbgkj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lwiuwnlx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qricjycb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3siddpkbs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pkczzsbi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3aurtcqhs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bznktslt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mznnexfe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nyeahlsx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ukztxgzi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ykvxgmbf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kyiladfz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pmneackl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yklpfxsu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qijxnctg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rtidwmmd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bloetkzp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjogauox.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uoleaixv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dclvhwms.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlvsleg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hufyccdc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3whichoaq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rqupwqua.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ahjcavkj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqrofur.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ujvphmge.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dszkwyko.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3znnebukr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fosawkbq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wvagcwpm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ygmxnjzm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ikfxpdey.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvhdwcv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rjegftou.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3adsfkyan.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lnkszghe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3swfprnci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nponjbfv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qzecyuyp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lzyewolo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fgiebckw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3atfjkrno.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ffcaizhc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oqersvtf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jgoenpxl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hixrbbsr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnlpkotw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rksivups.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dmbabavg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cwtyhknt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffjrumpq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sxqoiztq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mraignrw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3oscsebpl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dshbijwk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kafszwyd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ckhbxeqo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3osunwrxj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nshpdiwn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ztjokibu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rwnxngvd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3phdgsyce.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3axroaxpm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dascwtrg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nfuhzpli.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mzkgbmqc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ghhhefuy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzelczm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hyccvorv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvisbtrq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3szzycawz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xxcalkyr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bqdavdpl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3klmmjjhl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gflvvfrl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oercanms.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3llgdoojj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apkkbklh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wftewoas.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gfggrdqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3sfcufhnk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hcdvdhpx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uzkvcdte.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrfwhec.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3flxjxeno.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mcxgwfgy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zbwvegip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3psjxhble.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uupulxgu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3prdshsgp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bstiavbd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pszlbwpj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bhlejxeq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sqvgtgnt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dpbgrkuo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jibmfnbm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fwaqdkwt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lmkncore.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3progncwl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hylicjmc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jyzedgpz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzxcixme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqqmcph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3khvqydsq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfenrsyb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wogyuqad.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3czrpwlww.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hyecsjkg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3emlngufn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lwishtrf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ebuypxhk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iheyxlpa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3slzmzmrl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tlcevwnb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfbiehua.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vyhufldp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3taetjbgf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tctdvori.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nyhejxjw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdbewupn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ztjjeebn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jillhvis.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fkjrzodx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xokoifjq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewrelnul.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yaecuiru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xkpnbqjg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tziwcneo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wvsugrql.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fvqlmrtr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wlwjartk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xoxljuap.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cdtubskc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xpjimaop.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qgwmmenu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpvjxqk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ygrztxzb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxamagi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqntfjil.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qcsbjiax.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3djltsbos.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tbkhnhqi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nocqtcfn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bxowkcik.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lywzgiuo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dcmblwhv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuobexmy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chzquifx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yjgblbia.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vmutdjpr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vfrnsusc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zwckcbiy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zdkrfynw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vbmrvqgt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pfnhzoym.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lnxvgtvg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sxnmrwkv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvnkblta.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wsorkkar.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hbxectsx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkezcfwe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fvdyecpw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3foeyveje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yvbkqywl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bjocrzwz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hefagcgb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3szijmbui.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wqksoohp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kcdquqlw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vsrdbcid.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3theytiyj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdotjkvl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3udymiwsc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qyefinsi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cfhhaoht.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lqxoiukf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pzyeqiyw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yififraw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3obrgyhfr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dobocprc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lvxqffsl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ytahcwkx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhgnlhj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sipqoeyz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nnwldxtg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qznksinp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyuposs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpkktim.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oxuhzorc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mlueeeza.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mxnqggvc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bweldbmw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tgvcekho.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3piezpoox.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3otyhjpwv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zoygurgs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xyqwoove.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3larayqqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yiottjhn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gekqtbgq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ylktzill.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqhwngor.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvbbety.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ozodxwvx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rmntfhgu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qezvagoc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xuxucyvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pqutrgeg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3eadmogvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3grbocywv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmuvvwna.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ebvdtfjp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbgdgxy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kcrwtdvo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3arfsferm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3orecnoes.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cgcdybcg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qysxjync.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kwcerlth.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fokybvqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3roheladu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3suqyoljn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjvmzuh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mdnvlsje.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yfsznxgu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pahwtiml.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hmskevng.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jvhdjeny.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pkakzedm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3snoazxvl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wycohabj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3twhemrkz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3czegfemn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tswhhlve.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pcfffxvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvykctlf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oegblvgw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3entcsgdy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3puptaeds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aewvrwny.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qtnhonoh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3axyonzbn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hwgtumfe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uoptnogi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrzfvlcb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bzevxkgv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3npiapsdo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tgbkkzfj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rymyqrff.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kquzopyt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tfbzfzka.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jjxsfcou.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rwgmlojl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3oxfgdqlg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gpvcadga.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ldadhegc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wuhiojml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgwitfw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhanzig.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nixxukvt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hulifcdg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ivevjstz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bdtlglws.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3levvkpsf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3drznfbyx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bwesxcof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xdjwsxzb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yxdyxtsj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yjsoijac.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yyscpmhz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aoajosvh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ecryzhdl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3vhvqgutr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nnvtqrbj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nekotvvk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fvhvknpl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bkcxxaco.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lqmesmah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zmerfgbe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tahtzqox.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jlzoichy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bwkafvfk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uqiohdry.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3segmjsty.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yxkwrsij.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lmbqxpii.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jrwjvwne.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wfwyoqah.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gypuxkkc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3grtpkgii.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wzjcpcmm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yahnklwq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3newlpusu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ednpamra.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qvcumtqm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hmhdrmra.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pmngmouw.html


<!-- 参考信息 -->