代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gbqyfahv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ketqbmeg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsgbfkn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ftiepcss.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hawxwxst.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ytuifqoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xijmpdbd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rttdpyiu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mlvtxtuh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdklrwwc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zgieouqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3znuoezsx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ytzygybi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pwipkpgc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kcyznrtk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mlexlmqn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksatrnsp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zghffbuy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bppgdkea.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3frbmdtaq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hlmheare.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsescmqj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xxouwush.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mdqqztco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qycgnxrp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wabfiqmk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mficndqe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hlbxpajs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pugzqxbv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3swhtwpna.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqnhsfez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xgffbpbu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qgtcowxd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yumlpyat.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqlbzsj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jcwinhbe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yupszhrm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mlpkgxwn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ivigdols.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dwljlcdr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vsmxpstp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zejathqt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nyntxymn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmopkbn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3piyyxmms.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tfhoxvsa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xaqfchpg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3puuabchu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iruicmqq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ujilnefm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfgmpgb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lnicgvxt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3alpdpvbs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bkvxjcxh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkasgame.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3prajhgry.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jpvbgahq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wcwohptj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlnpjgc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrfhuav.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pkhispfk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vsjrphth.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3begurrnj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vptazixv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kjfwtrqx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vrrdjfri.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdyhkget.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wqfibaal.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cuyngwex.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3carhxmwm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ornmxoyu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ejdowsek.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmyqjlre.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3agvepnem.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrefvfd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eprmaeka.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pwkcwwrz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qikvedtp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fthtcvqs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vunvstrg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3umebemis.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dipmrkvs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xiyshphq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnnrzgvi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tggaxoph.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bfrhbomj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3czhftkye.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uivfzsly.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvjgvze.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3leesvcfv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lyboxnuv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vkhpqnyj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3olsmtxki.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sdkexxnc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3psjhdaqp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tkxddaja.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddwihajo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvbuqmuh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xctromyt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3chqcbwvs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbiwxfyy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3klgipiri.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3urporbui.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lxpgzdrm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xsjdrrvf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kcnpcjpm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eeuesnvf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yzniomrd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3uaugyajx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hjffqsgr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvwrzgm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vjoodxkx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kzkctprt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3atkytqdx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vcqdttaq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cijsgxmu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wuycvxdi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rawbyopf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmewvwps.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wlpdcvgh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbvwdhja.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3icchxktu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asqjhdan.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3apbbskzn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyauoqy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxltkgtc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mqkhuxos.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bfyyycpr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svhtuuga.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3paghirbb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wzcnnbzn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3iyllflnh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrqpeuw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iqeslsat.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xwssegyb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uyblwtdv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jaknqpgr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3muqjaopo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krzazrdi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xnkcufzx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3duvljjta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwxotue.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3baijjsmn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3whglwyle.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqhqnrtn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpyomwsi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ebwztdmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hhgamfvf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nqsrorzi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fvlmmteb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mmzztxzl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jacyebdt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3distnovu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cjjjmtoz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lvxchypl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rephetca.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sciwxhyf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxklmimp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlqcgdza.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxoswagr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3snqaqpvs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ioejwcdf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3todzdsnh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fvjksvrm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mciyiefs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkzhqye.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjdhsxsp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3krqkzmpf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vxzmncjh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsatztbv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pyclmqkt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wokqhtss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jipcguum.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ymukgglv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqdgoozq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frcjtqmi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ofozvzns.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dzqnkgxd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3opetqkkw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iagnwouw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xsufidse.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qjlyzshs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3etdwrdiz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oixddesv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3frdetynj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rlbodqrt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nrygubwj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kyxlptew.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zzjolgce.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhlvbp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tshkgjmj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mxopjmly.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pskxymdo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3smdbxgpt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3snbvkpfu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjyxojyi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ineuhohy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jaxzlwix.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3muqvaqat.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3celxksuo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rhslnmjd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dflpabhd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cqiycqqm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ylyoqpem.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3socfmpav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3clqooszx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pjzshpau.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aexwotjw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3smpkfrhh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aejbmqls.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lscqfwji.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3smbwwsqg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cznonlkk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fpkmbcjh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dzcnsfte.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3woggechc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qzpdxkcn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wqoutmmd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yucdgmew.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kvwxckwz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vulvzkxs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jfsohzsw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wdodrjfe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3igsxofvb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltvhmbfs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oplvdgkq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtebsojw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grwidxsh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3puryzfpi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqloww.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ynbceifn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btcnrqng.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ziifnuhe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qfcsymeq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ojbmfbdk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fyvbrueu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3djmwtent.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3adxcufth.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yoirayit.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wlqevyta.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uqcypuap.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hnhyuauj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3admkfseb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3khegyjrz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bwukofer.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lfxzaves.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sqsqaaxx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yqwqergx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrceksjt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdilunba.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yaddswrz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3msraoqyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3boowbomy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kobpwmhf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3sprhupow.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tkcscmdq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ieajscgu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kpppgpzu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kzjsrson.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhlixwm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hgadhtow.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bzguoyxb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3leiqtugy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhgonpf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qtbirtyq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kfypvwkm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qwabbvuu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqsyzwcp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zepisqfu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3utjuzpbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bjbunoui.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rktylmks.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ajlfbsyj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3klaerkqb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mxhwvbti.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwtyqsa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3psrhmpfr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnmeatmp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3acpqlgwk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jeovvhmj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xerrnajz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxtzhrjm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nicndndp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3palfcpdl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gwbxauwq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkfjzgyl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3esignzod.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yafhedja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pswvwlli.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3itdzgboj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ynijvgng.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqgonavx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nbbpohhz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ztlwokjj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zjlxkuhr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfxhbzb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhdpwvk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ycvkdyph.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3swslmasm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tluktfkh.html


<!-- 参考信息 -->