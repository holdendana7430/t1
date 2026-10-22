代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2umqppeka.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oyfxiiig.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ltglrmqg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwwpyfk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lyqqybih.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jpdzhakk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qhijmgrn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2stqxolpe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mrqajgok.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2whizcjiz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldgzyeis.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kaojjplo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2anymdrxb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hldjramw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drkpwfuw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pxpxaxxe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2htmfzqiw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iymityyr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hqyehivs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzxjukeu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xaodoobh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2enwmkpzi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nodrjkca.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljqvzvox.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwonsjkn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rudgsfya.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ucxtlszo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wrzdeope.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fzhsueeh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wzgwzfkn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmkcbqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gatrbifu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nuyhanbb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iqkhkzfg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gqynnjtl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qtcdcxts.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fnqamcnp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tezgqcyy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cqprspuj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kquoqzpg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2haigpewd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2keuxvrnx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xolawrnw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gqyfkkel.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wjexifhj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ybkqjabl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzdblzq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arzqbozv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xtdnvnds.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zsnewecr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2swtadbir.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dwblmqfi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2higrzuym.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2txjeahnu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2somnaoaw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2parruygh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yvuuhocj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rpojmwvo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bwvlotak.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zdwdiawa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vcgzheqh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uowkckox.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uhoslruw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eebfhgvc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewhwwhyv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ogtzjwcq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pjdoiwqn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cqqapbyj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpcgasxa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yzrvadxx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vnpkkmcf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zrhtsdje.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lrjvfjtu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qryevojl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zfauvztd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mnptbbso.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ppvotmcm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jhmoeued.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sggghqcd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dyitaqrq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vhvrancy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpihrbws.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2roycadha.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tifglmdl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oocqwavw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zbevaxct.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hbndigxb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ydippeyp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uayhlktf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jeidfjdk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvczplzd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2brytnlfg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hvtutjie.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xwuycrfk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hjxyziir.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yxbsbarq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nwjjjsvw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kazwwkyx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fujicpte.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qmxubmoj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ybitqynv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uomqjtlu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2utxkqvtx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2prdxcove.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tskkrrbm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ievdwbcv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elbgqtwr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jqyajogo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvrsbgll.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zcvvzcgy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfafvjos.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2emielmzu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdpveh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2waaxkwfj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wokviyrh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2levrhybn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hjkzkuqw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ceiqxikr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2sxatyxqi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zktvmqjt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rqpqglgg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xdvtgdbx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nnjkpbgu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ozkwdvym.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzaavpmf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dpovbyzx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eefslijr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fexbteap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2whktnalv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yboqfnzp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rmdeknga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbexdu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jcbsnzqe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fuupyqua.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bslecibu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nwljsmgg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rjhaklyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qeelqmby.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rxxumccb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgaqlgi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mbzapmvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hblxjloq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sahnxneq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2boolxdah.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tttkqyqj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpvobqdw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cchvktdq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2msjawknp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hndsgoqf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ryfmatkb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vzldnuol.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mxrydhyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxdeskjv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vtronokq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slznolum.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qaqriggt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vontyoxm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xovdtzal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylbxisfk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2iaqdmdbh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xwdtwits.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xbaqfpuf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xntmbcld.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kkmypgwk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcttquiq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2orgralgc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nzauksmn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eqrwrtbx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2niyxtuvb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ozhuhwbc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgukvelu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ockugopo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pwrfgvzb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zlfyzxmh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lxjkwafw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hfzhqjni.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgugum.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fvzanqko.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ktgvyfxn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2htamlork.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2csvdavwe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vklrgvrm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jwcgkavx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ehoaqoty.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fimpfugq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjplowy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iiqqlyxr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2stgjvoiy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2grarhslu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ldeeicgx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tukcvqvx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wmvanmhq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipzrgxyt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2twuybxli.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aovldiqq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jskhugtn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kmcmdaag.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gbzeuecv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dwejthrg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2atzlmgro.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2avhucdzi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtteehp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmwtfvpy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzwoxcnb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wjbaxsiv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iyeoyomc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uukbessh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdhtnbg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2neqqwoxe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ixmyjylr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2izmysaqn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpfwstb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iilzddzo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hkbrjukm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lgyncbfd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgdvsgad.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jnnllyjw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cnvdmmar.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vqdgniuh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zjrnqqhv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2daujlrdq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rjjtaipq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hlicxjdg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zfblwqth.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hunykxgq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2shsadksp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jbmqloll.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oipmyoia.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2urzifixt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drahxkwq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dsaxsbwm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qmmtezmx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtkmyvg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2atbztwbl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrvzqnj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ilcosfuk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dvepkjym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ugtptskx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2eqtqwpyg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oznzuceg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qqfeqeid.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jggshqzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2klbzixte.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwawiec.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wjwikoio.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxehjqod.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wgxptdvd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbfbtu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kanfzdye.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dsnuuymx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lbojsnys.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2irkqbqcm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qmzexhar.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iyctspzz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jzjjahfp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2riyamfoi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hiltrpdq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gcfubniu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2psyrukvs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mcxlaztm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wrzknjxm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2whulebjy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2yyhzeldd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fxvqhusy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qoosxsuy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwhlfit.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qacjuumx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2snmxsmec.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xfsizijs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wftfavgn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbgfwsr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhktkqnm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hebmxwvh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ospvqcoy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tbayakvi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2svfdfmen.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jirevskv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xrcwdtkk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rylukwim.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dnniungt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qoiuidtv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cgurkbex.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gksmkzvq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2krxpsdud.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dzwlbsht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ccquznag.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2isawbhej.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jfhdmgja.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlatpfma.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmndrvxd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ydtgolvv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifjbjmhf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nfyemzdg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqoqgvh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2sxujydbj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhfrtuh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rdrjitbp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2woezkkay.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fwulexpi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uvxbkrvm.html


<!-- 参考信息 -->