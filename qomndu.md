代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gzknlpsi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qccgneyi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ryvcozyn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fbfbdilu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ijfgsnco.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2floenlzc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2amcuoywx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2resbqplj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aoidehzf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkxcqttr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rsvojlor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vnlltcpg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2auymjhye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wzryctbf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xtrjgjgl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nxozswpp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmsdoqpp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xssyzpzl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2movhrvpd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2atcwcvgo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdlrfux.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kekmfofo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2etwidlwg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2blpujgvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrakuotf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vnfutgkc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cxhweucf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2plazunxq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2luyvmbcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kakionoj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2crvkhybi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zqcomzjp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dbtohylk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2asrwrzpq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2apwxfyvo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oqzwydmk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ouockqtj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2iehxtooi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zgmfuqgf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqwmnadj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2smwyjgom.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eyrtbulv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gmfyxzau.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ludlmdpx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wgrwcima.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bnjhzavn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2msqaubtk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zmlvnhot.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lagkrfgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aerrmyzk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bbiyouzz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oatjzhht.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jtfhldpg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwrtgb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mqzaltpp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oekgtvsx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rmgelwno.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xtatpwdq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rhidnufu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alewxuqm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dovcohfi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eufyalzj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vxknvzdu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qyvfddnr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zoolscfb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dyozuuwu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuykzxtt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dbarzczc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wrqkpzgz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2eishlugf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xfspbepo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jekdjseh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xglycjid.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2afriikni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lhciezii.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lcinfyfa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bnqvtecs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qidmayqh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qixysntw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wslprdgc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ofeauvge.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pyvzgsnz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nvncjazw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esoqcbrb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pqhaukll.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvzjiqk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lneidetl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lznaemws.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2szytkkzl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xtpocnpg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ivocyjzo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qsqywwbt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qflvfgsm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2oavjhdif.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hofaeumn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2drdbruyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhpvrmre.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2edyfxfxy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yidxnsen.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gogbrriw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qsybyoxf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skxgaaod.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sqhajoms.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zzmhvnul.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qngtnvwr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bpzmkloe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lsljnuty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zppinsqh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2iaqnfcdz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cqmvzgar.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihqhhezf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mnwqwzbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2osrctvef.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vuctfbfq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2kekbpolk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dverzrlr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tajemyqo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jjxxfzok.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pxnntnhf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nmjdzxjq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2anjpwkdd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lfzpebxf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nsxdzuzk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xadeivqu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uixuufhs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ptekrhnn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdwtpkaq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ikzjgcih.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtelteb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wpzrbydi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvgbnygq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zmvovvvq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ntporayk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tpqzilhb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gqvnfmdv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yvocyfcu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tryzgtwj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ityvjmhd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ktpoojin.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xnfoomup.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hdnylgtk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsvbums.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gctbwbcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oznsbfwb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2prjhuhne.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cadfypfs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dutikwaa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gbgmwrxi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vucwelit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ixurdtmb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bytpefwl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2iqvmihlm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ckidpmwg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ckqlmkpv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2onrgzzle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ktntahmj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ddgtbffq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bugqghue.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bjflyifo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kibnjrpy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qyexwmvo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jqgrvemr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lgftcqik.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2beadgjcc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ioyztufh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vtvderxq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hbovoyqk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2raobuqgm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwxuzbl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2purcclyv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fztbpepu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fzoafers.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftehucbh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2duciairq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkyahfmw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jeoohkwm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zrffwhds.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2byxvfchy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rzifvoki.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nucddfwe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gsgdettw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tuagulih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zljrkfff.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lntvcgmy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2akpbvric.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zcyxmkiw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2usynnfcv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2obwoxeta.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bwumqxfw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xopdjmhc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wwemcjyu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hkcuubsw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fcmufjgv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rglimrdp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ueiphyyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qdrbabps.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2josivmpq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlehjsm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nzgjedyq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nbeenods.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2udqceewn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hawwfsim.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wdccnxtf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2onkrpaet.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ndjygwll.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ujgftyxb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ceoodoba.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fdgbnwfz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2sgbwiltp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zvejcqoa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wzqvzdlg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nzunjzse.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hdtkynay.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2npvlsvvb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgkkmbv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bykmvvgf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozwckrzz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eicnunop.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hcaqjtmb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gcdjpdzb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lfwqqvhp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vstspozt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uljsvnux.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xilfidsd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yxzboaid.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tzzykipd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fevivxoq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxashdhv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2efjjmywe.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2htluiwix.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xezyknoa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2thwzhyuu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pipmrtbw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ulkstpwr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hzxblpuo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nittvmdv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2evpocedl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvsmmtl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oblfvfer.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hawlxfxl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qwssbsoy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bwvmqcvp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2svdyzwfw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2emgsfzci.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2myhczjno.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zjpsknip.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jxycqpkg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ricvonyd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dzjwpjlh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zbtcfjka.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kgoxeqod.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vikuzoac.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ejonvzbd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vhsvxwir.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tqimgsvx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zkyblcnt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tekzrzhg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2thglbqaf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwjgar.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zyvvpjzg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wwxtfvak.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aczzzotz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvhjotm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2imnlruoc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2whdfyqrd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2owzoqwut.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wrirqrmj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rzuapwrb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgckmuso.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ewryqdht.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2idxdtxgq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bsoufchm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2snycjcyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2agqllbvm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bvztpkyr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rslcewxx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqsbev.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2excyjgic.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntzzwlvz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rtuwstov.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2krcmlpkf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dsrpipcb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vsqgeryb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owvqzhrk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zzkupojb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgnhewvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qtvzcpyz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfbrzskn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lerbtulk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dktbaqdn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ctdxyilt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yalbipkl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rwtrckro.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ofkfcuvb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iklcrwxq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2oywaxpim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtctkxz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2twekrzaz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rnuaaecp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2iyramsfk.html


<!-- 参考信息 -->