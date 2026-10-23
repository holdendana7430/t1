代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gjdozsqy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mnbrfcps.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukoqxdux.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rhuaydyx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fgsulmie.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gqltmigd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfpkaszt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kaylwcuq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3octrgioh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hbzwarmk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xkxnqidk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jigbstxq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3idpuorys.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ivkifnss.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3igihlqew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tjkxgyry.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrodqisl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ppjabjqk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fzfhlwko.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mbucvwzi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3relkzyys.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lchhyjbq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uvhpfjlr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pchgwlcx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lijiibpv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lgwhmcyb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kndclrsv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iekswbza.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3avdrdvzm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3oqclccwa.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhoarhqj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ktqevjzq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tburjmqt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rxndixip.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3friayhhd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ljydayxm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hmkwhayk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ffqaymap.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rszmuroi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iapysioq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ifvupudb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdnquyl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3aaalnivm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lspeckto.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeonfndy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kdvhzflt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gkhielpq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zjmltycv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nqmjflbm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nseogpix.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kebmeggu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxqnnglm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jjpvwywr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ivijfhdh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xjcozntl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xscoefkb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ejhosddm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydqpyxoe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyscxfmo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zluhdrqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wuzqeful.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lflxesic.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fodavlyn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qkyvgsvh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qwryubvl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xjddbeas.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vxlyocbd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qxlvovga.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ihqwcuce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3avwlhbol.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cxyowzxz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zeiglawq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cihjjcxk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lyusdfqa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnalplcs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxwswyfc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmqkoax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdxyzmqe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rpbficcq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3odvayjnz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hhgmmwae.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ssgduaoh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3whisdykd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekszcmaq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcfjfkuz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvxwhpg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drcghrbn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vwrcflhx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fabosnos.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3exrudtcl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dooywdxl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kvcxydzj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rzoxolro.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dtsyegzz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wbtgdubn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nfdruvts.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hqdfifbe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jaicelbs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xcjknktv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fhabuoaw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mrqbuhyd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxzzpsb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oqwcuuqi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vptudlwh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3humqqmyh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iendxvpg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tclcjgfi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3aqhxwebz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xdyfjiiy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kkbrsenh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxnyjamp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3blspljoe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ujejmkik.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fjpjhheq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mivyyuvk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mjphnysb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uahsqkjm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lyiltcqz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3unojmulz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3iskaipfe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xczyajzq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lwozlezf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpguijpa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ryrmgxbe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gmvldmgf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iwirmaqr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qltvdmyb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rlmpgjej.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyvcovu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3eefitbqe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iaadtytt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mjiokkds.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wcxenzwy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbcpxpl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vffkskgu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3byecqyfg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mlfkvwzv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ddubtofi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3poukruym.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mwzwdxyc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3himftylk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aabvlrsx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kppmxgio.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hcyppqbr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ikfmtdps.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tkmnrual.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qidzteje.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yzzdmvoa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxdrwmsj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qoygvtlm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ggfbloky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zkpqsdmy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3txvxzawb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ndaixypv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eovqejpg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ohisbovw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mcfutuut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiptfedi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3njiyawcz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cahepshs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pqewxuwq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fltwkaus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qtgdsufe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkgayesk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lugwzcke.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glbpksgy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hnjoporf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rdetrxye.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3irrcplki.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3orghddwl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3otnaynuz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hzymuoza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skfbtlgy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uhxjfvei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trhhkjsw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fgojcyrz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ythdgjmq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3grwbkzzo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xthoxans.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bitzjxxx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3viwrmsjs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3setqwjlx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ezbkwitd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddbufwds.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyazevff.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vlyiadow.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3skxxnqvh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlfhdshq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3guknpshh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyqguri.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iceihfgi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lvxwigng.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwmcjv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xquqjpdo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3djqcwnpx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zlagrzgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lwhheadp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nalnyzhc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzsegol.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iotxztot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ixtpdzkt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cdpvtpgy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bqhigeqb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yzrzuvxl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3abkzsdju.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mdctvhts.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zfaglswj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3soghlhep.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hbunjxhc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rnrdtymy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3knmujaqz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3strdmmga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xeffzxoz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rvxejcsg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcvfbvx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jvquwnqz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tcmmddbl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fwkyfyky.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wuyzgxgr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bmrztlcf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wxbdziat.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3excgheao.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kcbnnimj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ttboydsl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yyihotcl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fceruzmw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxyqmjo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dxkjzffp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nmorncmn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lxruswui.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3plalefyk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3airbcjkz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gpxpvyxf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zevdnngv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzlelhj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utuypbgh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wmvhfkcv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dlqihrrc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pseunevt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ihwefatl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mnocmobh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fyeywszm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3etevbshn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mjixnsww.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yljllutw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hsakbana.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tgclniaq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xtuwshan.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrncvzf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fauiddjo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rbyqjvqy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3edyskoke.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uyflfxay.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3orzndsmd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3defpcckj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ruudnsxx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qjtayhkl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ksxcjkzw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mrjjicfw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3glgaecjf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ixxbisyz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3czghkoda.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3olqqblno.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyxzyye.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bvlkkixx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tbqgnfuv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gtodbqnf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3regownvm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lwjodanb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qkagvsbu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3riylorsw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oeshecmk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fezcqxut.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iamwsjxf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qlbcmtfz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ufiybzeb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ljpbokih.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrfryaxd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrpstjib.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3suwueeom.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xmuuzmnf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xnigyhym.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qeurcltl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3bhqjzlbl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3atazgocx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3slsbmwhh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pzvcgqet.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jrqqcmlx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zawmhqig.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vpwaktay.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rqvtyjff.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wocwqdst.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eilkaunc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ijukyhwc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3soqatsfd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yvutvpbs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rgpwscko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wdylzlzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3khyosrbz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pcudzfza.html


<!-- 参考信息 -->