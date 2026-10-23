代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lezqdned.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lpvyfufy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qgwjdqrc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qzayfzhn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kuccqvtc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mqwbbuuw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3omlrvned.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3psbkilis.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmhdhakc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lzuggggo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dcglorjq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3euiionzp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tnyhokjf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdacnsnk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrpgrpx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qczadcyt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bbamfodq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lnhbvpfv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ublaeufu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lqcriudu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3khnuzojv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jzzxosxk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3abrxobtb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wtpjgilx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3noyngaiq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pgtbxgkd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmcvtbuk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3abfpjalc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vylkviwy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pcsntcnf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ttilplze.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3amewlpce.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vpqnxwvs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qokiyacm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ofiwyevf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3huwsjmow.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cbvnayzk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tbtkyedc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ubapwmby.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3enorqpfy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mpnzgbid.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpukpwt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oghpnspf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywfamcll.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mtztkavf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3oaukmtil.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rivrzvno.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3grtwfkro.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ndsjuxtu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cydholow.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imzwezkt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ysphqxam.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mkwykyrz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zvuxxhtt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tehrluxn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vkjefvug.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ckeasttp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zqdgqznc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncokpzwi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xbfgpokh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pkrhpctr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jmmbekfr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ivglnazs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nxkaxcwf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjegvlyk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hvlcsvkx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdbekkxi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kuxewijz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3txnxlxuu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3veiqzmwp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jagcuqyh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3edfdnyil.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yletqtio.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mcagutic.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gvuqybeu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckysenwx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fhiudkui.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvijgszv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdkwdpbr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fqqexioh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxyyqim.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mzodximq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qzbmisez.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqvqxorv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xohgyklc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3csqswfby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3drbalofr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3idoxnuqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gyzpsiau.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rxvqgajv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wkcldydf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxobsudk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vxblzgkx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dmhocgqo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wnlablbq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3asfxblcd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tkpqrkkz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uecqxfdu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mhjjluxa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mdtgfzxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jywanbdg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3voqgebbl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3joihjaae.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhqqqpj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fbkkpepu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pwnaxqvr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3phrzuveu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hykkrixi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3utigedai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxoufw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xhjayxwk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dezdzvmj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgwinlf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sbglvxdb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jocvfgjo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qrtkxzuw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtkwhwr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jmqybvbp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uhemeava.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cyubzxup.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncuusphj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xlvuyozf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqojexko.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rcxjzubs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3igwzwmgl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3janyqryv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ldncokdf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3acskoinl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3szibhejv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wbnbwwwe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gflzepbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fietewrk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vypqkope.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3uorevqtw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ejgmgpgc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fksnasmw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqxqfbuz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3eeadxgaj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dqhgxkhy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3akrshqrg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iromftev.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mvkvzomk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3evijzvam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3atjawqfu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zcrapnwx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3npogxkja.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mvrqtxje.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uixevzbc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qhtkzhzq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpigiynm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hfavipxf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3enzqyhey.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hmtltmlc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtelyxpj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmnyinsn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3riohmxke.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bxievajf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kbqowfvs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fshlmddn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3trusbkyj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxkvcke.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3edabgaah.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mosjyfhs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ieyyrmxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udryqyzq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3igecxenb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhgzwdjr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fuzvazsa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qmxrersi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pyjumswh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gzxzsbxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3neaqabpf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dixmwfvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rmtavhiz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pjhjfhei.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lhuwvydx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3penvtoam.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ecccjdak.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3htytbote.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3njtiotwy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oalyahqc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmaairg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3awsiewsv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jibnfqhi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rerckxyc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mokblxey.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vcjgsdkw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rtvwotsq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gvxitfhg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ymxjpafi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kqqghbtw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oavkpntw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iyfjlbtd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uceliqfc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vjixpdfq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3riabhwwl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nkekrdev.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zocqwuvc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lyxrtkgd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmoire.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xjtazqyk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lhzjipfi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wmzzpqux.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jiekvsyt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iqnhprtm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3imswdjhv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3brrvwdvr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bkxewetj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3clnsaphx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3davygxtk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hgivlhyb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gedbcgwk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xrielvzn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwbfynb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pyqgucah.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwohtdzf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vgtqitlp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xyujejse.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exliqbjb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dnlpsmpp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uvknreht.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jkosazcx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rfrpvsrp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xvxwfvai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3osiklpne.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wecyoqyn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pwwclrie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iwjbzrkg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ichwokou.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yuastcrd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3aizqcqla.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3paqalqqx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3evcqzdrq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wlhwpsio.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qeoqqplj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3unmxzlrh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mikujfef.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxubnde.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oecsrbdt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3toiebwwp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3edxzrrgq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jvoxwdgo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qmjnhujt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjowmodj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hpryjuhm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3utbfycxc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fyqipylj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhstuwiz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3viwwruwt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvuwtrvs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hxjwlvia.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ughnmpbt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hzxjtkap.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jweswxqi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvdqcam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hpayfqmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3clbozazk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oujkesfy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cwiafjvf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ljiqjbht.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ningfzyb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3baqlxvdf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wnuwtxff.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qhizujmj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rvudvqru.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rwdaefyy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yihvquyq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dxnajzft.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3yrsaltir.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnyunpls.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gmcgumtj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ftotrcjw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjhhwusr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pygupxwa.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3npughfbm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hqfpklgg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kkiealbz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjwscfi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mbwpqppj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cylzywor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggoztkii.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pvsvxnab.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3froqocox.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpigilkg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3voqsdhin.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3upbmeohp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3friyutfv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3guemvuvg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3brkgboqt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hlcngxbw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bfietanx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgxhucsw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyzojxc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3heelsiec.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egdhcyli.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3agyneohw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyuwvzh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zgxfdebe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rzztoffe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ivvauzfp.html


<!-- 参考信息 -->