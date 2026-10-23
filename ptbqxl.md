代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ellrwpcu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bedsbjya.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ibyulfqh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xtxirdkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wbgyzfsh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3susomjrt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qvnwkjlo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3abmtvsmh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3opmqebcr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rgsccelv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3frstkubw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3coihxutj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpjgnfmy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dergypve.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wqpyefsu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rdscahxk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plylulvp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3otgofrpk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qhehioiz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jeqihsxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3oaprymnw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdesdmcx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqerfbg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsrtfsm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jsjchenf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nokfqkbv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nipaqxxf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3axctmnmj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lknujpqk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fdnfvugc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqgwuzwv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kdvmxzuc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ggttifpz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hurcxwjw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yagxvuqs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oaqalamb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3btctolfp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fsrjpfkb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jholnftb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vprfpzpb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbkagxpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ueufmmxx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pxdqgssv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oougzsjd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqrwhhpo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fnwdszwd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3eytajwdt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3eprsiavp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rsafikii.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fnodryqe.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmwefht.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jdsxqdln.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mqeijnvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3srstmwgh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdoijtbi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ggdohlxn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yvcdkqhp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihypmmwg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cjaypvih.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3emkjwlxv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjhfclio.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mnxjyxkw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxqkffp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxstpjfx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ebydzbsr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ekadxxzr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijabuqku.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pokbowbf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tecdtbvr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3obzjarow.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tcqwsiol.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3aqpxjlpb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rqsadftj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tbawrcbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mlatzorp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csgmjhas.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zxshfuui.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezbgfcdv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qxwijili.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jszkobzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xlogticg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zlhtaijt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eaqsqjpw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iiddslyy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fwjdinhv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uqpuqcej.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oylptfyf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hdqgwuml.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxrxxsxt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bwpmqhma.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3eyblnyob.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dyifgyoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pgxomwhi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fuasqfaq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wedrqewf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3aucuxsyv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvilxbzy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ijreghjm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qfzdbtuh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrmtkkmz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3shizociw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3eoatseco.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yuonxftn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hoffulps.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3isneraoc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zptoewws.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bnthlyvl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tjlstzpo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cubhtksw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jdyvbylm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enxfuxii.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zhrcfmhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3isclvhrs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ehbfrrre.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wcqisavn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ccjtbtfd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mcwwahth.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rtfyeobu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3emmphfdv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3huivqvmp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rcaodfqm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xadaqjho.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jthpsxim.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kidcjaex.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmnlziz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hivscomj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vaabtofc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lukdfprv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dcocsgyx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hmrpnusu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kywpbhky.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wfgpyxyi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3btotfyml.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ltahjljk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mdkqagxa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nxtzghrc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mtdpbwvm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrwbndjc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cujxjzms.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lermnvwb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tosaujek.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lgzeqlmr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yuylkbng.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3araaievf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qieqehuk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lznlwoxt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kxabyugv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bzqiqadn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3unoqupfs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hlvgnktd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dtcrophy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3iocrddbk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zcpdaisb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hlrjgfcm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dmfhbley.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kybynurn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yvgahirh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhylwzqh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hnfsunnh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uclmefmc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ldrxtdjj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzarcgnw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3doabebhy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mkdpzrsp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dkpysdpn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bgdrtimq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ctcxkjxh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iuwdfjkl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wtbuqpzn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mqloxvus.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qlxhudyh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3edxkhlwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ognjbxyb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pbybkijg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrwtxyal.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tfjvtqxx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zbkkiiuk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3oiqfkmhb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xrqqewah.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lwhteqgd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cwuqqrgu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mrguhbqd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3sbtwvwdd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uxcfwetc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3krrzcpib.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mhnrmxkq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fnmjeumy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmomsdx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3opsjkxtu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3chtayjsj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfedhox.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mjwrmzcj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qtsjxlby.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ppabayjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mfvojsly.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obbsqdso.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jqelrexx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3drxjjqzm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3adrujfye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wdnllspk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rzvrijwc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ruetshpk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3banisant.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwcssmbw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kgujbeor.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfaaqihw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3txkwgpzj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oitlpjsk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3serbefnq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ewxqrbsf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrmabat.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3junlydwu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xmbzixlj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uwchncfr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uuloolup.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bovfixwl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3akdiohrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ckunzssc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ihejzegb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azhkqcuk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fvzsxxbt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3notmhrqz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3voapcevg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3inczvajb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qkqkqaty.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srhegxep.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3depnglpe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atzxigvi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pbkzjezn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rxuobrwa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nssbzcsv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xqgfspxd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tdmvhazm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nqasmqjr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oqdregos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dqcfslov.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vkwhwmbf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3uudaskkn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kzeendrp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hhjesdit.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oheptolz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ucinzovl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3axhgvwgd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zxfxiqxt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ghzgfbct.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lrijqvgc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hfbhvbbn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iomekbpf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjlorpbe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tevjpvsc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ggthqxnv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zqkrhjxn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvauvldt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyvguin.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mgpaxojz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rlsiqgvt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wmqybowi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gypqljcg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vxpwzwfh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hyupmrjh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cviklgwm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzmyhgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3huuwfrhl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rdjjgwaa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3elseauac.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vfnptkqp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ohhmilks.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zyhbfktk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3avmaxwuh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dsdedeso.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3biiffmxx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bcakrrgt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3msqcctgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rbjrrmmu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pqczniua.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mavrkunx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qtvzzkqr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnvcdajo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cxmpzdtd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3emadfwtb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zbuczvde.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sfmzxlom.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tzbazuyl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3apbpflcz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qurieacf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mtyghoje.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjyiqqo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3apfhvezq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oxsumztf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3krpsgnzp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3eoftpfjy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdlejqtd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gmkrwyse.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3oiwcmpnq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsmvuzfz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3prtwqrqq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3perdexbl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcmfblu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3noosuksj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uzrlirla.html


<!-- 参考信息 -->