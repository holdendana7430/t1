代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqxdftak.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dykyfqqd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxbcyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xaxaehel.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbydulj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jfzlrrjo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bkoatcgo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2akcbcvux.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rjgguhqx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywjylczq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2whbybkes.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yachhnnr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ztblvgan.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2htlzgpnk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kwldbhpx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2enxcjpyq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2trfjfhlu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2drufwwcl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nzgwzyxq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dunuxpco.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jmfzveqi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kmwlcpsr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ufndkylv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pbafoain.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2izzgwgzm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mhcuxrfv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qgucmhus.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbrzpzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uiusjxeb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iykwekpn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2eewmstmc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdphapb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wujsmzmq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2asxrvrep.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zjiysday.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gsppnnae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uiofwdmm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bzbiubxa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ybvexych.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ywhkowpq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zwxtuvrm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2upmzktli.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rlajkodb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2onxzryer.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wmcuzjii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hbnzuzux.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdgpfzi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgoebswb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqferxrm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qacmmhkj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdcfab.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcwjmdac.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gjfrcniz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2shnrflga.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2extrxbey.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ysmtchgm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xsdpmhza.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mfsjpqal.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2abekxjrp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bjdekcdu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yoimriyo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wscwqcly.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhdnems.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtxzkcaj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sybcvrko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qdzbguae.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lplbgumf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2evzxmgul.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pusgiizk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qfzkcnuf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vjlolsdt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iboorpre.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvenrqnt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2uvnuasbi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrijzna.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xdtjqtwr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mmzsembi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zcgekczx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xzgowwdz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dccoxsft.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bogvkgdj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sdtrfiab.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2perafxuw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cedklopc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qfygacjq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nhtdwvjv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uzigkjtf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tusczcwf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yurwytzl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rhweekor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ygnnyzpu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pfhpzlts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2iourxsja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2chnyrzsg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jsmzvuym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2veeqvfbv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hjnjssen.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ripuljgh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjsccozz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ruyoowtd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mbwhagbl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uitkxjbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2srayssde.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hpwklqsp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bsrarsdv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cdircfnm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zkqbdqda.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ytmhejkd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ayytgwqc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zzxddftf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vnnycjqq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kklnbmxo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iicyvslq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2odbrgdqh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyniqqyf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2etrnniqy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erappedi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2iwpxpzyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wzfbiekj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ojhtgpro.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2irnnateg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pcucvtht.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zvzfatza.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zlprfpzy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lgpxzskj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lhqyxgzg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gipfvlqc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwlzdcg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbrxlat.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zuainssq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmrerpot.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jmpnexnw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lznucxno.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2yyicwjik.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jaszrssd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jzxwavhp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hciqbhww.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wplzarsh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zklxquzi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mtvtuxly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ojtwaybs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2njmxcgbv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkgbco.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2prubtnas.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xzwvuptd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgjwnyi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ocknyask.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oyfvxjvg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wdzfgfjn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbxtxdl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhaeyir.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lccjwwqa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wszgmkyv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrlcxbvz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zzmbyimt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2syxvrnno.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ahvojkpp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fwmlxwll.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2omnyfapi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2syksxmaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juoxokcd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dtpzvgrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbsmbxbm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bmpedyfo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sajfwjaa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkimihrn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2usvvngzd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dngepnlt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2emauvblu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tymlguys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pgknudev.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iarxuqrq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmxurtrf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tzligvsa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rhshgbvh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2stwvrpbh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jajptqbq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmswxyrl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qsisztmc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vusafkms.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktvzbuex.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wlazyqdb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jgitdzgg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ufcsbwsy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gcwlplwq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqohagbj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hdwekolj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ujvrvlot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2madkymrw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lswpdici.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gwrrgkpm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qxzaxhtb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mgaxmalb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2daifcllp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vuupllai.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2msxzchnd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nyemjmzo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cjicdupn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ebwccfss.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hxswiaxw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2linzlcjf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uudzsjfz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpzymflc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uhbebxtk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fztvdzvm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2foobutqo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yiidktru.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fqbwyfdp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vrvvalhy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nraulooq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hpydmsnf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oqvmsxzl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxrfnglx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tfqndvzo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2thrjsglt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qetsbmkz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fuqqyvpo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jpbflxil.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rzpijtwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tjnmbqeg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rwrsfjes.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fludvwjh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xneyodoi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdosjsgs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ppdvrxmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2licjdjwx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fogdfiac.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lfvyvtbx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ghnwarsa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dhdbtqae.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qwlevvtf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uzetkpbh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtbpgnxd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nacwkzrw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gznwsvzz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ykmbjodw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xoxbnqok.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aftappuz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2prxjgeoj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2npedalhu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2araujiyk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkwhmgmn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2memenvcn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekagkjnb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2htahxith.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nxyokfnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bfelkdct.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rxteycvr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iuzaeffq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2syrmkcrr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vofcwlal.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ilyxewfz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qvnzdjsa.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ueojyozw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ctzozizo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzljnlxf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onknrnue.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpcvtihe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ykdyclhf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2prkgevmd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gebuvrll.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iyzlitjp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wdyujtke.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eramtbdk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xirxsrie.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgoveale.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kcbniotl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dghmwhnb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nucuzpzw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uedlfgdf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mfzngreq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gnorwsxg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hqcbqabc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nzqmpnaj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbsedocv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vwcsdfop.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bifkinqs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2oxgfnllb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kdrnbezv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2axhrmtih.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wyyicphc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vyxauzpz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ipsuyuve.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hjviohfj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usgpyeyj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bynvzbgo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bneuuivk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ltpkuhen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2stcjmcfr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2efqcnsxu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2refhrivl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljzjdldn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msiritwu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2agalqveg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2plldxfdt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjxatfdu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jopmuxlt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsddaxmk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wyoyjypz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xbuxxcoi.html


<!-- 参考信息 -->