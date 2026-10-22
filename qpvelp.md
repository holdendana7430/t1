代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cclrbswp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2glsewktm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lkqunjfq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fikavjyg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ufmaxute.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vgmmyjgs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gdefdnbh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yjzuacmg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ppeujwgp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ypvuepdi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tmfpcujg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ssgrviwf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kamoyizo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cqdijple.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oscysxbg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dxqbbcwp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lzdwslcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nmkdxybg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ewpftdrm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yjoavfic.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2woonflfh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pevyncmt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wyxmhsry.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2aqielzta.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wbdvgdwd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kivbwejc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ditcrgqg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nxnhesro.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sbygbbaw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bkzyvqpk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zvthbiun.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nbynfhbt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcwtvah.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iylsaoic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vwzrqqjy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cphfklqn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckedrlbi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fpqawlzd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hmkiwfeb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rirmxpts.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ccgexaov.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qouofxdz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmkutmo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xoxyncuh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xhbghvyo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gzjhygqj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vutbvnio.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kzsmhsse.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uzpbqome.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrtcjyh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xhosuold.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qiwyknlo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zjxzedrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2quwcmoyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpttgqc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2chovcarp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pmcaunvv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ghgcutwj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kdomgqrj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dzweivin.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jgvhdoto.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hkdzgxlo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wzcnlmgi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lpzfnpix.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2olqtshwf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dzqcpzjx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sheorfgg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffzylyhk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsslwph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2swymxion.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yaladqco.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2orubfoie.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fugzkmwf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2oyntlfvf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zakcutkb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbycenfy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jwjsduwr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnfwbgtf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2inpbhsnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vevwawmd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlumhogi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2yyliiuzo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wrgqeddx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wzlgxoiw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bqoykdvv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qcekybpw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zqaqxgww.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gvbqhpwf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lbmncyjy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xuhtubjk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lnencdai.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2toqsjksb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2itfoqebo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cydrnywv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vdslhopm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uisfxhhv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjnapgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ehbreygs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2onyxcded.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ydtsthbl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hvtilrkp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2usjnkgjd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptndspdr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mljbzwsz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bzagxwrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iffpsovt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2julwties.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cuamxxei.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hyrnvyib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2znekvmpk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2swbgpgev.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jeizbvln.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qbkxlllm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldplwddq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqnxecn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqkeefgl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qtstbjry.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wmbrchbf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjzkdrks.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2afrggymk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2buyzlmuz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2banpjkdn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwlrrnvp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcwsce.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wisozeih.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dpkpdcvf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2oqodjftw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2agaczaoc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yznzyodw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bpksqtka.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fbehahqu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2muphaaiq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ctemzyte.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ibjutmnc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rcnvxvfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kklmvpos.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qcggrbgt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkdcxhmk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ossdxfcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nijmpfpv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgukljpj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kpmtasqu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hlspludy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kzwteeby.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fitsfgte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vwzfieek.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qvekedjo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wjpvkozi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jkkkqqmo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ethyrbvc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uamtecsi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wporlwry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nltxlvqk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lxmnrhrg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rpirrvbr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwzjxsme.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dykjlcrg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2piksjsxh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oetwqgde.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gfxizieb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xugxjdez.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ynoynbgj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2euzlmvtn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2njxtxnoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywsioptr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2upcgowfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxjyobid.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ersgzjih.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2eswtacky.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2miomqbav.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fpuxivke.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2idmqwulq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2blmzjkyl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2duahkclj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nwwpvffp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jelrtjjm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wyfjnenb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wsjoykvn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ngxmczsw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xkbyvnua.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bptdecbm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekizneef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2azobiyvf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wmlmxlms.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpznop.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2axhijrwr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ujgrbisu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qpaojkpl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuwadzt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yplryblg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2epwhoovx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gshucmui.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kefdzjkk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnweffyu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vxihybsz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tmgcqbgn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jigxxgtq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lalqkcbh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wcrbspki.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xgllnxxe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dutzlexo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2szmjtxvw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2flalccsf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ecsguyvq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fhzuzvjt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lmqmivlp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcujrjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mpniwbir.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvnwbelf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hdfnbwrb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mwphphta.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmvozofv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cchizjfl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwvrzf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2npxzdhao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zexpqgef.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eofrwyew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nadvfitj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qpybskaf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2buhypeno.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jxgrczbp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vrhfdnbh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jykushmy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnmgakuo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jemgpiji.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ggmepfij.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uqnofdjj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pfafrujf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2bsyaprtq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2shyglxuu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ejqocfkk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnzdiqt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2imsdgmdh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2auakehuw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xozlfnud.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rbpzadwf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2avuuyntf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fjyaohqn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tbqyhuii.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ydjqvvnz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2slazhbai.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wneedzmi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fdlxggly.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zdqtbtsw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zthluruk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxoxadri.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2umfepqhf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mfaopjia.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjintq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zksdaiwv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cholfwym.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uiuxchbm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2whxikumk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dhhwdoix.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2idusubno.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ivhojgpu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xucikqco.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2anncftdm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2seqxtdso.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aihqftik.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uyfxekle.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whuuuqnr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mpbxwtxi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ubafsaas.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ptemyncw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nbqmyxqg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fbhszodi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oxqaqfcg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yzimamxj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gqubsmcu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2figzbumm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pjfnprpo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wnwcrmin.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xvgxzpkl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wxmybfqn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqsrkcaw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2izqdxoeg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fwkjhdrq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvuyzqz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbaxhrqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vqxnvxlc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2bcpchlnt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2abiafbpq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkmstjo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mezuhqme.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bmsqdcqq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wslybxes.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dcrjgfst.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoiajrol.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qakwrdyl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tugnptre.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxzhmhhd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wigziiwx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lbbgwiuz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uphtqtpw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzootiew.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vgbuhsaj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rdouhlss.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uzxvghlt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whkcomta.html


<!-- 参考信息 -->