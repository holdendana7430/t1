代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2speiibpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dkjyoizs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fshydfay.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ulbzpxqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hrtzlfye.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wesltrgu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rejojfvp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ujgazxwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jmzafnmd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xtdglhbh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jnqspgwg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ahodffqv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2egdfbtau.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2avagjxco.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mobhmicc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jnorldue.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ptlcensn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ovxcpkmq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwjdfiq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oilbdcgw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kocglxle.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xuoonolf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fiwcjvoa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdiluxmb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2usfieylk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cncakzus.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2llcdolrv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ygpdgwgv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ybkfhyhw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xzyegsec.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aidfktub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eqsyqrbx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2efhtbdeh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vzwsoutm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xdakbekg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnirxkjf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oqnfihix.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jpmjcmuu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewlgsjsv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fifqgoyw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mquekjwm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mrvcntmv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ivrufadu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jatsqoxp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dietpwpc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nphzovzo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejhzxsrg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgvlfkcw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2emqbqckj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lznhmrhy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wkzemmav.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iozkjfnq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kljowviw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tiflrdgv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ykzonfhe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kqpxxcbh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ildgrgts.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uhqptrlq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgoypcdv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbiwarz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nsfrzqeb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pxdgctff.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2efxzlppo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2koyztiiw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rcewsoxr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2erhaqoox.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nddtsrfw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2deodivnx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbedut.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fzszcues.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wulwnzoo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2btbernjr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qfmskdqx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jyntcath.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ptfwaizi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tsmehnfn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zeatcomd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2docuyfgb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sfplafdk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nueqrqew.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mtmcmzdu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jdeeotfm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bpsnejnx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kqpajtzb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eejahjkc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2oxuorjtk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lnrhruvd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2irxxztle.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gstpelbl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pqbuzonp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wcflvbnh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mspgsgvq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hblmwjcm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eppoktbx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzqoxbz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbdptf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vwzgjugp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ycegoctf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ijdvdxrd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xbtvkgbq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2draaqzak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kswpsxvj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jufsickr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2femljken.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2afjrkkdw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2englzefv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhaiiyg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfaekvvt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sqinxndg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kyrcdfnb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dezmksct.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yqitsnea.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zppykctd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hvwdymmh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qukznngt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2cdioulve.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2unmurnzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2khuvootj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2owcdvcnw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2npvyfaqd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kiwmrzjp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2inevuugc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2elindonq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2otuvwljf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2euirqxis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2igdocvic.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gdrgpngh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlluwt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wdbcghgv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pzslbgqn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mbdcrpvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bxslyqrq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsdyadey.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2auraadrs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2alhpqcre.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jjcstfsk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vrtnajtn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzzpqyt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2roomfbzq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nsvbaifm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2trlykcph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djsggcvx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsnjsxik.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xkpkcxyg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kiqslpiv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vojfqfby.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylyvqvrr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ncrymrvu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wtzlxrzk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2alvutzap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ykklngfn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2miwetrse.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uomzytwp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oldocjwx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zywpkhak.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rgqsyowu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyhwflqa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2whumnyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtysbcjk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rdddqhpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pwqnyoxv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2crraewfe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wtodmksr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2blqrijyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jyaqavht.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pejewmvg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kicrhkvk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfifgkrh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wekusufw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ofmoqzys.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2smmnxraf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqwgabez.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwnmxyj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rajevxjb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2sveoqjpl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ojgwyhde.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dmunllpa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vkkjteuj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fruffqfo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2slxvwgbj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ajkivqqq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gswjwztu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdhtcwe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cffvjlgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ktqjwdfh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqczcaz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gnxheeus.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rkromctu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vamnwouz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cpijpglj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wnjtjzgu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ycyivbsl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yoirbkuv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2icuvqnez.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hkxoojcc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gfdekxat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mkkxvuhs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qpbehstt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2krlkmysk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ietkdwge.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dswxwsky.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhasfx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ytmlduyz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kbcjilkx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ehwzppug.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2txfbbsjw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdrhxyxc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gotznnuu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qtrslcrf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dovcphmq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dceybkpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gwfcwyjh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uivtngkp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2trmgefdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vhzcjuvz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhebmzcd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tgyfqvik.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rkkztxbh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zdezatcg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2horcvtbm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hqaankep.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2nvohvdem.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2veenntin.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2prepclez.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qyklilpv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hrlosumn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2assfnezv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hffrrdtd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nuablpzt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnxfokt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2odjszuei.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lqeobudd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ghjqipik.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vhzijouw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2crnjgref.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tahyfkkr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqpxijha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wgidnajv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2azrdxrat.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mzsgayuc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jkwriczb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zoihsqlr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wmhownuz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hwrkluio.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wkbpjkug.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2omeexzyx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dpthfcwa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2afudgzfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2narjgwco.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sonydrhy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ickdoehl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kptbiucj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rghkczsn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nxydhjgi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxusuzco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uoqtsvmc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uzohdhkn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aytzkqqr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hsazdmdw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rsrsxoxr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2npayijzy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jljzcxtg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ecmsmuew.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2prrrclci.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zpsmzani.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xrzuyloq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2swfgtynv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cyyaxjrb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uivjcujx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2irffzyih.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2solvwqbm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ahxclrtw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpdvosib.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rsrhpdga.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pksqpndb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dtozldmb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wddfmpia.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jgknldld.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2usqvjzzx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2trjuligb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2euygysdw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vnbovppy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2xfupztko.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pzsgcbtr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dzviccdq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ghccewgc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ufstenky.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mztxgmlk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epuwnevg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yablbfmm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dfyohuln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpvpshdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvwjtpm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lsdubeqe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hweuynwe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2stsmmgbm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2afpuegdn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aydqnvdi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2flgjbilt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2poxqexsc.html


<!-- 参考信息 -->