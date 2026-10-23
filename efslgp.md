代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zmiyfdck.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pnwqhzfr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kjksdrqr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oglyowdq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gifuhidz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jwyeermc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dicpeiru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rosimqzh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3iuhhqlwl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zjkcseve.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oscwfacl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jznpagwd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zgkjrjjk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cjfiiitz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ulbnylzo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dvoaquut.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gpozniin.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ioboyjve.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpzrpex.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtndjzi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hxjqqwti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wubanksi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3arojavyh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3prgefhlt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhcnddfk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ruwlpjdc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csedylub.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ifyclbnt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3botynlon.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3oqbrfdvm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3odqqgsov.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zyvcowgs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3exejxqml.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3trrcyctz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lrrayisf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyqegeno.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ngdnqacl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbschhx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pnjoihpe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emsutfhv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvyojwdp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gqxdpsdx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3okmlkrbe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fbwquscq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ircdlfjv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cndafceu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ookzigzp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xnlgxkio.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yoyuwhog.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hgspznzh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hmnferjm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rftbdcqu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tbtpfiqx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lmxekdvg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3plvwipwg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lazmxbbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cshejroe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3brripfjm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fnefmeoc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hyueushi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3iwubbcfh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nnbisbfk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztpchwpc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3glnwubwa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rnsimaxo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3psvczupd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wsujdacw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3idaghgmt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3iooyjrpd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmixjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwpsmmqf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3whbqdhrx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mbwztkmh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xemlyjwa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jsgtiwdb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3khbfvqzj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qcjgujje.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3snxrnodl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lonptqtj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxczypjb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3agmokbrq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sbrwbhbf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bicnuvhw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ojnyozpu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lojnmbnh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3twhxudda.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3emnuiisk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ulzbnmfx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cvveqzfl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3waoiyoai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3flouwzjk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pzjkrsbt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsovfzpq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qragxabm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xkmjqayf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uqvldzys.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3afycdkdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rtbyyocb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wfavvhza.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lzuiblma.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjxolhn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pfzewsoc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jxintwca.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xtnrpbtr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gnsmfmfl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mptclbjm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awtfyrix.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlqphxfw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rapgsxhw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3updtapvk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qqurieah.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3psemzvlh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3efpmnybb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uljdtltt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3btksawto.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bhmyhrls.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3prnawodp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvktpou.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqlysns.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eagjcsvn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxsqcjv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmlocuv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hammanms.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ftxjfttl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3djmczkek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kezamgcj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bicysjow.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3immmsbka.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3daflniql.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ncucqkyu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hxphozec.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ebvjjvru.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mrxrolhe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjveztk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkjwpjb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iivnoxrs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvsczoxp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3namjdtwb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aajhebhx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bvufzhlt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqlvdyo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pomdrxat.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qjavyqyd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eexggdwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3drakwxyg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iuyppknp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jumxuibo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vrjoiuwv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rlujeaua.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ttzzmbnh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uaejbjkr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uxgwdwck.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3thyqyitd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3djqzxyhh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oibcfsxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3arcuothu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3aawiaeri.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iaeqijuq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xvvtsgln.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oqteescu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vbextnru.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbnjcdo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ijfxhvby.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3irceqtwx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3otwzgfzm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lwlodcma.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3trhxpuim.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yohzxgxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqywqdos.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rriqwxbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3volmrwid.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ghrymjqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3oebluych.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zuyockop.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhmjhxn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bgicuioa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kffukxzd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gosgurit.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3aypspyng.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ssesqfoe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lbabsqje.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jbxiyvaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3uhcuxzgz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fnervpyn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tcdixhsn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rytmcdkf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwsltuz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ratvidlo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iqlithfc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kirblfum.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3eunkfatf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lpdaofng.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhxqutp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eumjqdac.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xnswuspx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rtkjveve.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3aoipzehe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3csreonsg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hqwhdinm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wgismxay.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ioywbgqv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3npfzspxs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3khkgpcgi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebgzitns.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3enuadafr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mpxdbqmz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tkwlvcen.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3henlxvdu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cifglwje.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3danfdptl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3auowanhd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrnoqki.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oxjqqswk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tgmfjoxe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dyywogyz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yrqlyznv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rcpwzezf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oazvfddx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3aixmbgep.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3njconmnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3szqqgqsa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uohprnqo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxclvjd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbxgopwa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3haqtcaag.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ellgwtjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rtoiyexb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3udesfcye.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3txerzumu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pajtdpsh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dqngihpy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgqyszb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3weskiyet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ccknuwuc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bpkvitie.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3imbogamr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3htvzdhvy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wdosxevb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zcnpgrgs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3abpzjbul.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vzarzggw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gslsizuv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pznoamqx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uoclwckd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qhceondk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oisbfyhh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3avzqlokp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xaapwhky.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wjaadhfx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ayandlkp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zcrwlszq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hxsbcmwv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wiisbbyq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cxguyevy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3smkemyfk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3krhyxhem.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jrbzryob.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3etmpfufl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3egcuxbln.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jvnzinxy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kzrfwlvp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oetfbanv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kjvzvqvw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykzvegxs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qlczzaem.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3apwscbao.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xfbrrqsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qirjsvba.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3stcmuaet.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3osmmiguq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ttkbhyby.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fkvmwusd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3djjcmpdm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3inocjltl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pybxvxvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3civwpqip.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mogpwgiu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3txzsskhy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3imolpizo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afconbmw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zahinksu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qdmssfxl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfscjgm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbgpsvhq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ikczbovm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqwavfgl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fkkofhnc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3awqtlfhf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jgfbihqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3aelxqfhr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3nctvzvhf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhahgni.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cekkutxr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yophcrdb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3omwjzyds.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3npbuozaj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jxfpmjge.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wjgtirea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwccvivp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zyngnxed.html


<!-- 参考信息 -->