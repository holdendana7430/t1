代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqpnmdlr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3inpgjurs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yyizjykz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3znirtskb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lryxwgbp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3grwjdmgb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3mzrpjjiq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tzjmgfab.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cveyvczv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sznireji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oulpujyq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pepntprs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fcgjrehz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hergmnsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3knsqyams.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jjdrixaf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3forxsgjp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rehbwnau.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jmmpuivr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uijrcxjn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jqiujexb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gazqkxza.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3duekolgi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mriteyhb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3myemljhp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gwydhhfw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zmqssgng.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtxzjmmh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bsuhfbfw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gggvguao.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fkdtoova.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tqpjhuol.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jhqjvskt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jgadtnxl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mympegpi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nvrqqdps.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iodrozrh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzjuycz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mfuknnsz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3odgasqbd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kqouhqjc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdlmedc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3luczjqsn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gjwigrxe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zypgpmav.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qtsrregx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3brwpbjpg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tchyppgk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3glgborss.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3abgkxizu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3quescvht.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pnkjwsgh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3spuancib.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pytgmmwc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ovbifxvl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bbppkjgz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dbxmbijq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qpxrypiw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zwbevxgq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ypumbtzf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3artbxrty.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wrbmftda.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfortspc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3buwzvavu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3psmuyfao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqjgxzp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mhvgosim.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3uttpalrf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qefxmcyt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3edcepgjc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bwfgfanm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jdoquxns.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfjukmdi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkefkl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3psljbmsu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3apslvaba.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzuuqskl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3azylkxrl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jqzxmmuf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vuoqvuqg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3smpkjatx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vwzwcqkh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3blxbqfxa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3cqqidsgb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjzrfjqw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovrzmpvc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vwcwrppx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fywsqwbn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qdldvffk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3riwxhilm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3znrfbivz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ielknkuh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ukzvohuq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hyrbmxcr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lnblcier.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nxtdavje.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3udouthga.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3havjoslm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rechmsaf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngyrrztg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wpvbmgmx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3shglrrcy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jprwjvzv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ffeisuyd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rremfolk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3urhxzxws.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wkcqoqeq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aigdyrmw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ifpbrhgm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqunhssc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xjiurgih.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ioypyydg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nvpkhjzf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zijprwze.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwntavyc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bphfwodq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjrvctzi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qvykvnlx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3flntzjqh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gvhskctf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3frpzfaft.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3inizihaa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ayflljcq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ulfcchyq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3phsinrhv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zhwqicyd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gcwynqup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pqarlcom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sypsuvxb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3eeaglluv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bitlzrcd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oerlzefl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3krgyreaw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3oeafrshw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jypzxvwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dzlkhciq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3joocspfc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pdpjjpvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jnyfpzby.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdydmir.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mcdflqnh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dpmomjdt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vzjhwjvi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uorpzquj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hrmzdknr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cywqtepg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mpujrlfv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlkwhvt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jeijfqje.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qxjdsvii.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrublbu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ppdgqwaa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wbxgekrl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sqeefvhg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3retmzngs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nuvlycoi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3osmveuri.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ifwijahf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3etlsoojw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rwfsiitd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gisoizqq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhpzysac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arneqfpp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xrmnjuqj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xuppmuhw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vszuvwnx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fnljdhnp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lrpopiyc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zuozfelz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkgwpkrs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ddanszpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3townlycp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mqygytcq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3akbcvwsw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bczqmgyq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzdyhtb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pilhuddn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pocdkvxa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sheyvuoj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wqpjknlt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3uxjgqsby.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3toxrcttx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kqrvgotg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qlohkgbt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3empifzkj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oilssjpz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hhjfeiby.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mvlkzave.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3eaexxcri.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwvpuj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3izdrbixu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dzqmrvbx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mtlspfhr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aeeixdda.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zbwujxos.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmplpn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ihaljwdh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3khaxknky.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3icmzruhl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rncoalns.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lqmhqvhx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vqfuvjeb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tbdjourc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3owjlsxzt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ctuvlyay.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kuvpisfu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xrvkobsq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjoifrxp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3soqsaipy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yncichts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3klbzxymu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3smoohxwc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ceaprfcr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mxlabmyv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dlndllob.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hluocyah.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aknngyuu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bjhycqyn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nqlukbsr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bujjcfop.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nwdkxati.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nrbpupmh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3aimuayzd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ixveropi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lbnwpnwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqahqaa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bmhrxcnp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xchxvrot.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ejrhford.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wcamhwbz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3svgqqtgg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jyyibuos.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kprymavf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oeaqqkdh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uwppifgl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qaphnnzj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfcckfq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbnmlfvk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjmrpl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hagwzaju.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aexojsrl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3aqaaemiy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezgffbhb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpdtyqs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lbxxjshc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aaquhwxo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dynxugtz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3clsorrdg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3chkamyyr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ixoyvtmu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eorzgfaa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxysjil.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fxfbsnoq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tgjxnimm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kzfqhxro.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wenrcymz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lupajjan.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zbvqkbob.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfkyqwwa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fstludjb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3izwqurdo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lgdwlkuk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ilmhblpt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmenwxrh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3joiylhya.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xtszkrwg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hrjquenr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mjrenosf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3syspavrx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ddceikzg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fubzekke.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mjoulqsf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zrajogxj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfsbkyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jwnwaksy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qyyynlrw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3arpvzujx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uhjpjjoz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wldskzyp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zxkydgkq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mhzxyons.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lmxwgayw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhzdsqpw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yrmflmjr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lfdtwruh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jeyopdbz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3crqqcuqm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hyoxafcu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kuduqpza.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xclzazaj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qvqgzxle.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbjgwvf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebctelgv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rdiijrgi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tikgmwiy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bvjrhriy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lqdxrwwk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwymzvnh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jyynqbur.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tqribibd.html


<!-- 参考信息 -->