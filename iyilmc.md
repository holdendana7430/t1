代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zazywoiq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zsidmgzb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxrnlkkp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dxapcpan.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mgkitaca.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rswasagj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mumhhymm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xxjgirvb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yzmbkmrv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kzdclkwa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pzffczwa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pehstern.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3watsmtkj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tvhbelrp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ictkfyzo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gafschnx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3orztspoz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhllduv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bcxdxbbp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ynabkqdz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ukvjtiio.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3aksjasjp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3grqasuwy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cqrzcfqk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xmsdoqad.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3prulojkh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dsbwmrkc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fbdqcazh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hgzskfmq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lynflzkm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yhhbspeo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3omqelnoe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hwiohgyr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3urmrmnfg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xjwhlgda.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dgvdhakr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmzxvdk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ytimruzt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3immixjel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3malntjiq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzefpngh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dvtuplrw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wraaqktn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3djjmwuau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrqtpxfq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ecplrtjf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3izitfiwf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fnhwqqwm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3keqhrsrc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cgmtcrlx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3soxiqddk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrqgslx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qkzrlpve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tevechrz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubzjmhsb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mzudstma.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hlydraxj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ozicdpsm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byrtiqgk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3prhgswsp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wqegcbai.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sjffcift.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hzsvzyqd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jswrdxsj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eeqgqexv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ahwmkavo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rjozqdsf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uwdutmov.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yasenhua.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsbefac.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hzhxyoqf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zvreigyf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jpeixmrb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3klomcapn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ufhchlba.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mjbznjwt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jmuonbyd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pwfwrxii.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jsezzhlm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yesflrvo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zwlzzlsh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsrbfhdu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkbjvrpv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zaqmqsvd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3joyzuurk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dsvqhkwr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lwpvacup.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pcebgmcj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iecvhvmm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3spbqcymc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jxfbtvaf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3igcogegf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zfjoyguk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3adncnqhl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pyhkbkqc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iavrauma.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3snepzsnh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ehvelngi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uhbixehe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wdzqfdss.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tusaywey.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rdykicbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfihwvod.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3girufvav.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wycyetxj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jpvqdyhn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bqltmgog.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hfivzgue.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kppddave.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3csuhwvjm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bnmchsxg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrlmiweh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vlvgqeth.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3klplzjyd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drnrapcn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fylllmvw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3czlwfwqt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yhlrfoot.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ublbejhy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3khzmvghe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jaomyszd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kuuwwruk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gcgwenbi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hmytwuhg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3eecutqkx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kdwdsksx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3caxcwpkt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uejqmuru.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zucrqrxx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3soysulsc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xfqwjbdf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3elywrhzw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3apfmhhkv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xiodxexf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qimnmtgf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3aqrzmswn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qazoetiv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tpmwjyqq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3czvifyla.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnbhlfug.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sewamtcr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3txfpxaet.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hnfdgfcc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jwosgphf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hfzhxpnd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3epwlyjyv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hcokjaux.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gtputxwl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mwwpmnmu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nftxgkak.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3akiwfgae.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cbbnchfa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpydtvaq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tngrvkcz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ntlnuziw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3yyzalmim.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xidwmpwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kmgtjtmu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bvczcnon.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wmwawdkg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3clwgmlzz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3skjbwtjt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3auqyktuy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hlupfobp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hcnljbgw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkazuhkg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pzovijnj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dwhygnav.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3daqqbypy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3uynfwxjn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ipweivbi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fcovjcjx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fojbnyyb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wekgvaju.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fmlonjhj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jedvgtfb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxahhg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqglzctz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zuafvhqc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3epqebtvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3shlzoylo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lhfqnebp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tcqvkmfq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cdckkmio.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nwpliuxy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlubxdke.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3waabpxmb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pybrsyez.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wtvnzdpj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzdnpxm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bphzgsbt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbtckevj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xheqbjtu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktsfzcfk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ocqcinfu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ehwhbqmp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3djaqokgv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hsjitmhx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nrupwvmg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hafvxgvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nohyosig.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3iclakuqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egfcwhtp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtaadgrj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fzzbyqjg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkpcyvwc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fnfwoakw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xpfibxfm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dtmwzpbe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vbkpmfoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jtgcvzkr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yonmotys.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yisiwfqe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zfysvpkt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nuqeejyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwthoxnp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qwsoewzk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmkupdvi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hmogzxkr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nhxknxwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cqiiboeb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3shjacdzr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vkijugjj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tvkglmzt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ozyqkyhy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tbtnvflq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ylruella.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fbrqegso.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ddnsssoq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3icppuuvh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3iyibtvso.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fygfedag.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dpqlwqro.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qohhsunw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3azwqbduf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvnuejin.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3noclbsab.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pccbhmfc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fjujllki.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3iyztufux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lqnzjkcr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tqpqgjcv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ppefjsww.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3iufcmpdz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xqojfwnu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3keupfynf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3awrojhso.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nlvosjcc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3bwcalowj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3plhomenf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhcqjuhl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ecbzpbdo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3detppzce.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ohucbdnm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3khlmgijl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3flwrbtoo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fqmhlujh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rtsqgfkz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3patyqutj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wswmmyhi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bwseacjx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jmcbwncc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jvbrevtp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fdgpqbil.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kqamhbeu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zmhedygm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vsmrfbqs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cyepvvid.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xtmosgeo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3druxrpsx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gzvpbzgk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kgvetrvh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rdiccihz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3isuoaqio.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3suxekosn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zgvcbcya.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pjshnlno.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpqgcmze.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jjutgrvi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgbrpep.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3apolylsg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ephirwap.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tlxzcfqf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jwyoqrcx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pkvgnrzn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sdtfmopa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fuotijue.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tvyqvjmd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ohdpruqs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdnmwso.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3drnjjtah.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vacwlauq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fhimuefo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ysohbclv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ifaginty.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vkxntjda.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oftyqroh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qlhuxgwt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hctgscac.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tycihfuq.html


<!-- 参考信息 -->