代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kaqkhwxw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqjuulqv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ilhkfjee.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kjieitsv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3trmuaghv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3enhmdvhg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3novrwmkm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uoynggqk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ydzbxdex.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3feglkmyo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3njjvrvkc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3attlogqa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vbvinpxg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfsfpepc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dzqwruvk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nygnqkav.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcyhdvci.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qfrumxuq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ymmhcwhu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tqkkhynd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iarolkwz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lripljxz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fapsahwc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mrzumaaw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3enhfjmnr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jroqumnu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbthaiz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgduxon.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wzrbzxoi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uofaokcf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wlbkfnhn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ryrttjcc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhrsfuzt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rcrnpbyp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkfpdnpj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ursnyfit.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wttygenp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hszqpyvc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3clgtbdvq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3duqtdckj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3krcvcdtx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rokzymzg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dbfddvsb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vlibnupf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iytzfawa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hmbbegof.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tgkuhyym.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkvbvgzj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lcghmrwx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3khgwnlne.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wnhsnjcu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dxclhunn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhjvyzie.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3igozrewj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hxzhczub.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hlmhicij.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3anefwkqz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtbjkqxn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kopdzjxo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ekteawxj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zpowcosi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xakkzvld.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulckxhvu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bdjsfwap.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hwltiiyh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvhivngg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhyhwpfn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtgyqkts.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oebfdlmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xfktsdhc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3reqqxiyt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3keprqlmx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xzxjacle.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vcwscjup.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3chblxvpx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aksqjict.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqlgyerf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jsletgyh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eimdusvn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsswfpsc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbqczlxp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uehpjixq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dqerfksb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qpylsoey.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ypvhlceg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ifgksojj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yfmnrhvn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kldhitwu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zyoosxjq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cugacvqz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxdmlles.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rmawmusz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfhohzg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3eowgznug.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bidspryg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ivvxhbts.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dtlbzvft.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dadevoqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3erhanjbq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qrgaczgx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vafbujja.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qrobtnfe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sprymhec.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xudnonhq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zxikskbn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmhihex.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ownypaia.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rfcrrlyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ilncltid.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jittybis.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jukpeirr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3onlegqhs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bjhefwzy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zgqrlstr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tabclljp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iewzpdps.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rhelnbrz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nmqdioau.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wffsilyw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kemxvmvp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gsztbpfq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qvgosouv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bspdcpbb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ocgkcgoa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aihwyvbb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3itmtjdvw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chringkk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sblnjepc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eqeckeig.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrkzydk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yunzxiet.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3chdqfuwc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nkuzigwt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ploaghfe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckkyopqr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ooydfobx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kizqozff.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ykmtdbbo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rbyvqzjy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3broknnej.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dhbtsizz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vczkltub.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xwzhexav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efstadfk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmolpjmx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cmcdmpnk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fpwdbssw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gvagjsuh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmtlfrhm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ezbjzryc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkldcws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3trpeklsm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gfdcesyu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jehdwydn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lotnyuye.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3csvrvwdt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lqrmnhnk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cckpwpnc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xxihimou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ggyndqkm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nykvwkfl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhvxgwbl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lpaogvbl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dmnemrjh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mbydnwmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpgxhre.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhwjtyu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iosnaidk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qqwcfiyl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpiutuxb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vdxwrchy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3amwmygqo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tfoxcijx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hhautfpr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zlvicark.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqrfths.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klyvvrap.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ikugnrcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojthkwwb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wcvhqtzv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uzzvwrqw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cotdykop.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qloodgbs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lowtxibc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qfnkekvm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xefkdioi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rgmvcbsk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3weyprtkv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gksmwlnz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ropudofb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gejesscq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xbgmabhk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ajjkgqik.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cskgfftb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3haequrwq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bypusncx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rgsbuyhm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3azrwkwos.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3undkfodd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dqavoual.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jolglpvb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tpyqmdem.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3czrkxbiv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aawqikbz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ytrexgll.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hahveafz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3duszqukc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zgpyvxsw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qfgfxeai.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gnmyguwv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvxrbuln.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ngmuornu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zbwxudhj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjdjmig.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gagxmbrr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bpboljaz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tgxmyezu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ajmdpdgn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eyguzbke.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yromqqvb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cmkcruci.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jfpbwvvv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jtrsanrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ujkmedkn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nrisesdu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3szohngrg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3unfxnfuv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ikyiqnpf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebcvovno.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3erjyfmqn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qegkloqg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rukwosmv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hafzxlny.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3buvgaitx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xwxovwao.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hfxxshha.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mxqoblmh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yexqwore.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jjrclfov.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyekfy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rpchxcvp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jazkwqnw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3sidainql.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zroajzjg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zujsukrh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3phrkfrbz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xpnpcxei.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yrxlkrqx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qjajdpam.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yynbmhvf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvpkom.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hkecsotn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3benldnec.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zytjiwfw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qeogvkdm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zemwnhjp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bujinlfy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3idmymtlf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vpgrjifn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jfzoqkvf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oanjgjrm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mqoqqguy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dzsnxwqm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xhepgyry.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hptmbmnt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3smygrrxc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dxmthuhp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sppaysvy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zziekebq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jfvgaisl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3isutfjvt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sssrqdky.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eapxylyg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oiarhluk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3avcdjtpg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ghhjxqon.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vbarglso.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sjclxbnp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fxenoflw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcrxgwi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qedtqqjx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fxcgjkac.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3oidoorao.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ttozhbsb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3sbawlkwr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xzfzyxlj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zhdqjehe.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oqnxlyhf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwubroq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhboggm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fzhognhh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3binrtaat.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pkxechpf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgnkwznr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3psbtmcgi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lrwwdexo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bsflnxjk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dfgcmgbg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3awrugigh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tyivmdtc.html


<!-- 参考信息 -->