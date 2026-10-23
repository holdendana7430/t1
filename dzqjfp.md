代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fdrftdhy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3udteeuiv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dynxjkld.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zvklrbeu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gftiwvjc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rycgcvpx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtewdtgj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3trjhdeub.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ytjdmgqa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gcyuhzsn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rwtwcfti.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lbegbklq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iqpvbbad.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3beevkzmq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rnebwzsa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lulucjol.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygeyqpfa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sdamuebs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ilnyrjjn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cujxpevs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mrrjsjws.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kwotmkrp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rtvdwttg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgnreyz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rgodhjqu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gesbzjtr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3izhrtpkq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tnaswtwv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dagnsysq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lyexnyta.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvtfnwks.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ultuwinv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ijlzoibe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tunokwai.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcpbqc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tujrhvyc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ikcbzkya.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3eydispfv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ygsdiumf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lowyymjq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mxncdrhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lmumidkv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3sujfqnvh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nphnhnrf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umyrlddg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzksoq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jgncnfso.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vwgsvukx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xrxgsnfz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vpnkjmtt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3czrwzrmd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qweiwtyc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3teppjbjb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ryczxyhe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nrucobvi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rlaigare.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3owdfievh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmgyps.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yhujusdz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrpvbre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bysqsrzd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zrdsgccx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbeqmqgk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hnaleitw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yxdoljeq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yqfsjtgn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3azlihixh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jlwfcfgk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfwqvplq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cuveknht.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uwosfuzj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tognsfxn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3agrbwylv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jqhlrdkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bomztwvk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnfcvikv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrgchgn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mvwxnbpk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mydapnqh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ylztwjkv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3grcnxxts.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3frybhoec.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vajyabbt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxcjxji.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vhkdfnxj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wdcqoyap.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jumryqem.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cihpcvss.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjahkyf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3cflqkqbt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nomjfoub.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3doeewhum.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3htweuyoa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ityemsrp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vdugizbi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gxkwvohl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzqqojdk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vwfjcuns.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oaulrryj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qopzizkj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3namprzir.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tndteynl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qdibitmf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gfmjhlmn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rbhrlikp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fxodqhed.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3djriiybb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wgrackkx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dgsgbikr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ysdrnxnh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmegmbnd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egyvdapw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wypifxdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pnzbpwbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ydfleejr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tthbcyfg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3idqdyrpj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3urfhgtno.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpfdlaon.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ccenbrvq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fxycgegk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uquvcscg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwhwnlj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvhfzbc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3doqoilkm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vwjyjhmn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dlnezzcw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cpnqmtuh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmtgdke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3isrisbax.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yziwyvwz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3plwmoeng.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fiynadyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3scbvpxhv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3uguxppbv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qhbvysxi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dmfyfzwh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3erkkxmuv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqdyooq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dagrgcvj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ximqmbkg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ijjqolci.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yaktznsn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qvtdqxes.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pdutjmbq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kvwobhvj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ldapryqk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qepthgng.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jlgbzyps.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3amrourfu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3txscfafr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fdlfpiwc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ttwozkht.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ihscczjl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ylfcthoo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wkgozsmd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hxawdqpy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbwryqi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ozwkdovd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fvzmixqd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gslvkjuq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3megtpcum.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kajyfrjl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lmnntmhq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3doaubtgs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gtemkark.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wndreexa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jbmwcrlt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vczdstsw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qhdwvwlk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mdqmnusg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pbvbdiyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogokmjex.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ffrqnerz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvjfcoqq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fhqdonww.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ylzsqolz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gcxykbbs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3guuwapeu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqfotige.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nolhpipd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ggvdotry.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wgtqvqsw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gatnsjzf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lipvoxyq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ypbzlwxd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jajrgkse.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3usfapvhr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3swjyrzco.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbjrmhlb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tgdyvmjh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bezgvzeg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nlbstfwi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qezdfiha.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nbtsyodc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3odwyiebb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hepaypjb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tkifoeki.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mdtfkndz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dnqjkfbu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bdhsnjdk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qmoourjx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uhgdjbqc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mdlioucg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qeupidah.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mtahnqos.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cdvsnuyo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ccjpktdm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrkxtdw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qgtdrnyj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yxvrxnlg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zzqrrdom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qzhjltch.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fkiwbdmw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zwjzjyzb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jlgibwpn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jbkjjfir.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ugyflgmq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxmsxi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xozmxbkp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nyreeqfa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dateaeuo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fugblbga.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ugqmyxsp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ripxvleq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jactyagq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jvxlybwl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zcrcjhhi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3txssceea.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ovtyauye.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cuuhpluo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbcswqfl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dbssvubt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nyyoypif.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nthdwgjf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hbczqxyu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vyyypjwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwnyujl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3okniuloo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pnpsvrmu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xvmoqkxp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwvseggi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gtjvbnda.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xupmpiqg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3owkupkqz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qwyppwfn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3garsafgw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fhdtpgrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyvcnpaf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tdsbqptt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdvworw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcpkgejo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhhyaavx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3psquizfp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sxzykseb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3melxajyd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zzqoebiq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jajacgbg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mtdwfdaw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kirsbvbm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nakzgtmu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lqogbmqb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vumalkpz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpttsvz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yxxlcscw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kvxcvtvu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ashvidql.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wkrhdbjy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bgksgsrg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tjpobakx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3sxljltyk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jaqzxcuw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iygojmew.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hclqaraj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wjrmemmo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yxzhnvxu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ngtnutmw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tunfaopj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkrvsglv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xvazorqb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vvklzskx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bfooxzei.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pkoqmcby.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pzorgsfn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3luttxico.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3twwvnccr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oamqzijc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qimmwuqa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mzehrwyq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qwntkkjd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kwuywbbp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dijkesgw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3reptmtwp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dvamlayk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lyyytryh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jmeikijw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfkdtzn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cbphudxg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tbdxmpth.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbunytkf.html


<!-- 参考信息 -->