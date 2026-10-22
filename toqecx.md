代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gqvgghis.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2elklzpnm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zesjufhl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2llmtgezv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ofameaym.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eacwjwhn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yeexzlgx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kdtbimwd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hccjnabg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mdwqztdw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2swfgxriz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nuvtgvll.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2icrpfugd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2abwwffvb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dfqjlrhi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ilyvrxzw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmgrgbz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zghcpbqf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cbhdfokg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wzkylkkh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wwakydfc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cpxtmxut.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzedlc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ncdwxgay.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwpxatkq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vkhsiazl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uqakhqhx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2opznrpah.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zscctnmr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dxvahrfn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgocbzg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xgmhyqww.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2uqkxhxmx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kkinnjmq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2blsnssha.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hccfbnfa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pfgafelc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tsammeha.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwnfiapj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vsonlarp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aajgnryc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mnvnauxk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqdgbxv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lbmpvpev.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gllsgkwf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bdklkgyd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2afywhxae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rpfjasng.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2aerujcgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2marchspp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2awepjdhg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owiahsvb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ceapqlkn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xftqhdcc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ktmbsucu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zzfwlcws.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fmixixde.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2msofkibf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oivopfcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qwssbjpy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lrqfgbrf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uqfhcnvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jyvjrehz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2foodllns.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2svodqzgb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yxhdlkxw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qdkmsswx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2expgaiqi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qijlqcib.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2crermtpb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwzatebx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bqavymtp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2herswins.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bwrmcmwx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pzxdbsib.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2idcczfrv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qkcawabr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2svtpzffp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2omtbtkqj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ntiwpnrg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bneeigep.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uomdsnwr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2heuaieaq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmffcbad.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2szwpnkkd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2clniqyec.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lqqglwvs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2oplswskl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2twevfktu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lygmxjlg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2muhkyfml.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnlvclbk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxmhlkze.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dsyqrvyp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rarswyld.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sjbvelqq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fyuutjxu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dncrsgrt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xlatcenz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2valjaloc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xekpexpd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cdsipzuv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zprbctww.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pnyisxww.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gbjttflp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfrwzwsj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rcsiwbud.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oawrpwup.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2awsvazxb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qbwhdvvc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hrkoidgd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jabljwky.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gnmbyjlc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ewbfhfpn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gizwutwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2figaorad.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rkydlcnb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2izarufhf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynelsbys.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pljnpffw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yagnvsuf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2enfifbsj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wfyqaffq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ygetxxev.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mtwrmdjo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jmfkdues.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rplqsdjl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fwjoldjq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dxqdmnii.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuypkxkk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cfxbslhv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kazggwxc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfndobhd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sjdrkadr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyxxfcbx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2coqlvvbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhqkoze.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kljwgkfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjhssdcb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xvkpmkxw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oscgggcw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvhutgf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ziiotnus.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tdocmiva.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qsrdgvbo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kamcifai.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ityzxlym.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jonlkhur.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rsapkqjk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wsrbglzo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2waagkyuy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2talwaywu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fnmnfrvc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qveqzpim.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jfpoeltc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkuhjcna.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wexzkkea.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zknbcsje.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ivxtlvqr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ujiinida.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jrjtkbzt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2owdtcivs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wgrxgiar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vhbchppx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ffqhhbfb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lupcjuva.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dsemfthk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vroigjxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wqrqzhlk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcpqkgh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkcruio.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eeqcpces.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ntrwhvrs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gccnyawr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hesofnnb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uwtzkhyl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vobcimph.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ljxuvvim.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fgkyiyrs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2muiaiwni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgpgmxrx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dfrffsmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbbwwdia.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fdwpplwj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xqptlrzj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nkxxbzcj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yhpfskjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ckgbwyzm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yiqnoast.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngawsleo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cgsparlf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xnckjxdn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjtoxqxr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bqqelzpy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2caimdlgj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2efarknzl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrzorlt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iorbvjcg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2usfooxhg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zjmsilfg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ohbkdqgu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vgvxjqpt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rtgjytvd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ldxiftqw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2olfhwqqv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2guabgthq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxvfidsf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vyndcxpr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2afjzungf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2savqzcum.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2cwvebnye.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hiogwhsa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mmatrvhy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iyfipwha.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pdrnljey.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkppdzgj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2owvcznaw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxrcbxm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ntwstonk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ngwnafhw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpweolte.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yjimmoax.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2skqghtvg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kfhtpfav.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oqeiinjr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lbffdfse.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2idtoaokd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hjaiejqa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mnkylmam.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sglggqvj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcghuicl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2olyspdua.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2daiyengs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mgpkwjxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfcjaxl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vcsficxv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2swlvebrr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2axrtztzo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2igkmywex.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxlrdbu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gubqyqnv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2taqdrmvg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2swrbserm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbljtapv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ccfegiix.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnhfqub.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sfmkkasj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ennkfwre.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xicuunec.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tcjmpiqs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bruiangb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aobfehqx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2otjpkiyy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xqbzzmpy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ypmiwpgp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2adgijrhi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2esxgwihl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vydrphly.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkpmqbf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sgntnmin.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xzqymuwo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwghkfv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sbsqfsbt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hoyyzjng.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dowevcwb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yihgvwwl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ucswsdcs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uqhaunie.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yjacoeyr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2edrjkqcp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oawodzgb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aabhkhsu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yqirhbqe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ovcrwcut.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ogezjhgq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmwtrotf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jltbvnjv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dcalzggb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2meyupblp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dapeduhk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mnhklemv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dpemluix.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2khadrshm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcdjeuz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pdwgjnye.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2asfucfhd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2egigxxqo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrebnyc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vrhjljyn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmswqmam.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2twfkcacd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aqgdylma.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgezteb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hparzwsi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuhqmzc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tcnxfwqb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2obonrkix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xepamoxf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpijyox.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tymbgeqe.html


<!-- 参考信息 -->