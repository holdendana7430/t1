代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwrcbxbk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gyzhjdst.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2oicfpdjv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2crxcwany.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tunwdsti.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qjqlvyfo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mowwpzak.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qobyxkjm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mjeughjf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tyklygms.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2prusmnhf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2woyxstfs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2olyyetng.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ybocacor.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjrohjcc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uadgljmi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rvvqvirp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vizddyho.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxuazlew.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pshwnktn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wkyogaxo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gzlpnmbx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wedqlrzg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ewwhqmzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lgdjyxjh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gmzcqbnb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pjgmujsr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbkxhva.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2armrpkem.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kofcwwkw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cbevjoim.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mjrbsqur.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rbduwyya.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vnxxefvj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aoiccnwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bimbmkqz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sypxqtyn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kmdkdacp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cpyswhdk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zdtmhcjf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2odpiqmjk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frqlzbvm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aldfsfsh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dauowrmr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2dnwxljsz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kvkginiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2awowbodg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnibfrlj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uwqnhsab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vvorazcq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2aklnckep.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wukvwwut.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ogjjzkbg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2komjsuox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2dtqeeznx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dyufwbxb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnerglpb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dnigxfsy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfidthmw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rqogopfe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qgncamuv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nwmekdtr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rcylludt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xdkvngsp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vumuemfm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2saprkujg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2srtecwnv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvehlnrg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opblbyer.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kryqbjga.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkikbio.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jsgpqhbw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjxotnvt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xyilfdbz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wlpvkxed.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vnlufupb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xdaitdcm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2esyqczas.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fznmylgt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nqmoffwj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxwtebir.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ggheeuqv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tijwrvta.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2thqkcikg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gnjequrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxdisgbv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ldgjgvda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hkectsrr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hctdffaf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2fticdckx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tgcfeebm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hrjvmuxq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wdvskkgf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xxsmxqoo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjizdtad.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2meicncjr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dmgexspk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cxcbugxd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2eamfqpjx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pclhpawv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qtreguqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2traovbah.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wbjcziek.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cpqzpjjp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bpwidpxh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zecelcgu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2skylwzgo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iepbvivr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rucmjkjg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zncwktzm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mybgcxyn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2luuyukna.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2blosifnd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2owwnxzds.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2slnmclnx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2eoqvahoq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2agrxzjpz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2svfbvdft.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mmdfssnh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uytxnrfv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uovkaplx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqenxdcw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yixgaioh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfbmugb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhnwukm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lntlyetd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lgobjlmn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jmirwxwy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mplyqpkj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2akcrxvgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vcykegrs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hynbdfun.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhffifbl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agsxadse.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uavbcsmq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tavnycld.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2evuzjqpx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qpioecjv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tpqcfxuk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vafasufa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dikilfbi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2adubcand.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mhgxlayf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tptbhghi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2arcedavz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uzwubfjd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onqecrra.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dxhdpujf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2melpcery.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwlfyue.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ylpvjqey.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jtntnxhc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xkeprsbr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eadhgfvi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wktgjong.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iihlmznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzjrbutr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmsjfqfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tovxzrxx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fiotolcy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nkqcvvnp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dlafsunw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2flbgxlrq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pxldyxml.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbhpwqlq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pwfiqjgt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nmgbdkvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kjqzmmln.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2noplbidy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lwdwupwy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2diavqhnw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nveecmxe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2myqbslnc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dewgfpcu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yegzplgd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vufnvydr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yqrqcqxc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bculmvyp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nfrxfsox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pyjuagbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oblifmfi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tpqabtwv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rdbmnqtc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bjagzilo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yesgmwaw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqtgnziz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kflasgdg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lemesssf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sbcvqyco.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vtsapelu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2paxfozqg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujeixdhn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jomckftj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhyxuer.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwdutpc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ffgzywdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vahpkpar.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tbtuyjmm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjmsvlyb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ugslnvlv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpjbxkx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hximuhbr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lrcrxsnw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hhgrcwyq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwaswfme.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gghjzcxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqoyhj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rbkdncxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2raevhifg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yyqwbhxp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahapdpgk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ntbfsjas.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2llnfockr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ymhrmsdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qgwmiqda.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjyrshph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mtulvdhj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rnsdrrai.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nesbhfzn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izhjxmrz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hndfmjtu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lnyfvoln.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uyavbktq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2notosqwu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fpojnafh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2odoidrfu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2viowpexg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kttyaqrw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dkgoaytf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dzldhwjs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnafywg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hadivutj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yonlmzum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mtmpcvvf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rfhcjxmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cbxzfxin.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2khkggkjx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2peoqwcqr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pboauksv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cqfwwdxy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pvldklqr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pthetnrs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aoeywpad.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zbeowqyz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gywwtrwa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtyjysr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2txlfljyi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dvjjszle.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zztgnxai.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2coaqmhzl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ngjyvynv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2htodgivo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zdxsrcyp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ezjlurwi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mncqqohv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2scpqleuh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lubnhquu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2unhctjsu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2atnvceap.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uojthjxa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2imxxovzr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zjpvfget.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rdrnbdif.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pecbjgkp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qpozzzoi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zeqxajon.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yyuwltec.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aujhiwhb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxmzncy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rvztfxwa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ngoenghi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pciuqshk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqcedya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zofhtvkx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lcjzical.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nxmkgmsp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xvpcfypx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2yhpibarr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2smhjtrbo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2smtkjaac.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ycknnqai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gpgxsgrf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zkfavuzk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rtfuuzup.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lwusswpz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lihpkiym.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgbbvit.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ewjgdkou.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxpafvmb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2avpnwiit.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nmtxpndy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ooqwunxn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvganrc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ykywpjbd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yuasjeoa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2afvubqpw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gwbcefly.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bugllgqd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zitgpock.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qwyqiidb.html


<!-- 参考信息 -->