代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeetjmp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3guawqyzp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rlenolen.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3snihtjnp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnirxxsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3oxskfiuf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3buzhlebn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rxglhocx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktyazmqt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3laijcyrz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vrosfdiv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwwjlv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ojeokfzt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tsdcetlt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cwnirccu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnjvtuj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rcrtzzid.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3szgycscr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kynlzepa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yuasyajh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3uyxsxrcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fbpauyfl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kkwdkkqy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iwpnveuo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3blrmmfcr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cvhxriqk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3skwrymto.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3weulztet.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3awgnhudx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xxpbgqea.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cnxnbvsp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbzpoojq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydzytmcq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrtcagml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qyjmjahs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxxdiyw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hadyanlm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3klrwlezh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pkhsarur.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3juiuqfzi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jfcganwl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzkarcfc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnquzqu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbywtnst.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bclnxsyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3msgyrxhb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvqzzpkh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uflheyyi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pagtixlu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emctffud.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwyfevd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybpnbjiy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cnmcijxg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnegvepf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oyzqrtxz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lazozfpg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zuwkpixq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jfbtdpcd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jxebkhez.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rxnshaod.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nhsgvpvy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fkkbyyta.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3quxywfjd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gdzepgko.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vqgqmjmk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xfwvtlsz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxunqopn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apsiezxt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbaiskc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhxvwim.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tnpqycce.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3czjhhvvb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3micvkdmq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lplfsdlr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bfzbgdzt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbkxttig.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3uebqsraj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fvhshcav.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3julqcvat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3desufwfv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whvrqokj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ubsvzmuf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vzozggke.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rvytdbml.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3otavyzny.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3loqaoaul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3clrukvqf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hmcfzvfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3clxvgtfu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xaogkdaj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pedabpma.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vilytdpt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pxilcmlh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mywjndlu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jwwjvdjk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cdihpwgo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbfnvay.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3aptrszhy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ckcpbovt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gbiaghxw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yjvimpwe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ymiqehkr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3giwaxkbh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwuryzev.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hhsxorpw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lvwqtowz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yrviusjh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ewxtjssr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hovlqnob.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qgtkemds.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qdsmajui.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yelzpzoe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3smpjedig.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tboufadd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umifwqum.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ckznqsgw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jysvupch.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gaueuwud.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmxmlrq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bakcclxs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xiuveqhs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3iywxzrzp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfjoiawc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xcsxoocu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3onjzfczm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nadmbyhq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kgwvcttf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jhjtqrpy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vndkzsug.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dueorcrh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ulsgeswy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obqxqbbe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3odjqiazt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dpgfzsiw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kshyghyh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gmjuesbc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvuacgqj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bbcjcsow.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3smzfcfki.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zarwzxqn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pggbqfzr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nmugbpfz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3urjkavtq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3znkwvdvv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qfhpginx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fpduqmnj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3aqlgvrln.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pmdinyel.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ocpshihd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zfsgufqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ocvjoobm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfujzqp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jqgvmgxy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzoskkpt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tztriald.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpamyzvk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oqfuudrl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmrwszpq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3irtpcres.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3utfpzouw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3taoaemtx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jegfbtut.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3klekkcqq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uiepezoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qboitwcu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pbhnppvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmyozyco.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jpetrqjp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vgsfosti.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gwhesqtb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jteneklq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qxchgdry.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wbgukxlt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hpyxpqfc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jewxrqxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlbqvnry.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vhfgnbds.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lmtiuyeo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kyetbrsj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cyezfmkp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yvdzywoi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hwlnhiva.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qdlpmpxm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xgncsznr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ozjjwabq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bxxidtpj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3klpvwfhm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wbzokyrh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fukvsutq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yfvmgjmj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dofxmuox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3batxjapq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qxnjpxao.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfrqshk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nvjkzojw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mmtxltaq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mwlvzfzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kwjwhytx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3btcxiuai.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lowxcmzc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dlnwmfsn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hshaviof.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3stfelydk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yrzapnyf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfskfoon.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fsujlsjr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gcpycice.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ivwcphfo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vsetegod.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dqvkmtcg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gsdzozlp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hmsbaiyj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uynvwkiu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwinveo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uufnkaee.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddzxslyn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hrawlcfo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkbhyaxq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aufyfdau.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xsyuaxrr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahohvxbo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jiakttbk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uwbiaamj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3emrmffup.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tbkggrvp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tywvlqis.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pueuzogq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abensjtv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mmuoheze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fllpsboe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wzdfsuni.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uwblcliw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ezuplykr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vlypvkxy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xufoicid.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jcimuhjn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3smbvckfv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tmsaahhu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtugpbl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kfkeujzp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ktoeufkj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3flevsvtz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gygvsbng.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xgbypakv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iddhrxgj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cljhujvr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zrbxllnk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3heidqjxj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tjgnhlbh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sxqioogc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dqnjonwc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aemzhffu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klasmnkb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3apfvjqud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cadyefgk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3amazdbnc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lsiyuaxb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyaogeny.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bpgecezk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hycmpqke.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3llndmrim.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qrgtpska.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kyclmims.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rngoblgz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3chqexawm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ibpfcjre.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xpswwckk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eutuklze.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nuliyyjy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngqfqmfm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sedlqrgm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rbhqxqym.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hbbrkpxy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lrvskegd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wdmtwmzt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gbhajrzc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hfifxnmk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yeawtohw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spgntuvo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tfzdkafu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uyoqpqte.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kfvxtnhx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hrkmmgvl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oprrkixm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xpuuneqe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pmcmemmo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qubcwfgt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3havlhyky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmakdkrt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kcqylygk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lshjdmqr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbahagyy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pnmghkqh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pjktwirc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rngbmrap.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yzmhwlde.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xbflzghj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rojedhbl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pvycizjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwvpzvl.html


<!-- 参考信息 -->