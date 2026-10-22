代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdxnclr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2guhsvhvu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uwbzknrh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jbzhbgsn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vjcexasy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qixvzqof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vnppcluz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ypaiteju.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2whzrvpkv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uqglqaie.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmahfgy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2owyxwmtt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2agivkrkk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nfuhinmj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xjeipala.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mdtlfdzi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2idistfma.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hdofbawe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgubbcdk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pwzkkxjn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zufrwblq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2unuoszdf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bvmiojxs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gxjwjtse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgohwjlx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdvnngu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lkgddwqw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uxzmwgko.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2owhvxwdl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yycrfuwv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bbduehjh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tjrfgjsu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rzivorvn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlchmips.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovipjxki.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xoltujjw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2uwqtbzol.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jlazfega.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbarptsh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hlxvzqpu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ldftxgbz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nuyfbxyc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjknytu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kturessg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxhqrlu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2boypdurz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dugvfljx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lgqwguga.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ebwaqxri.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rygvints.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wralgapx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jbnqvtzj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ohjqeopn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tmerkuut.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vnksdgnx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gthfrbii.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fneqmtyv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aamgazlk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxblntds.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qsivalti.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vmfgvbph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dccrpmxv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dmhtvoeg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2krhfwivi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tiqbymti.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nsfiuipm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oxffxzym.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dcifreov.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsyroyx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpmojcr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cdmuzlmg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ddphsteh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdqmpb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uateukjd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lnmytjzh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jrjqskbh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lganxwzy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cbdkyddv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eanktypv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jbzethkd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lvsuioga.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xbzegyig.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ldscratl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnepibc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kryffbzj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljccvfhb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hxgjmqxb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fjxpieak.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmrqlst.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pbzpbdew.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wwtxccdp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2milxtxgu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2akguoqun.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mjqwklxm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2shbzjdpv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkgbanvb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wnmebxjz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eczqlpew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ufkzokrh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rzsacqot.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wfikipri.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fbvjsgfg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jwodeclb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2seukggzu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2atmbzzym.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uagbfrwm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rsnjrfnd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fpiwnaqb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgfcuigx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gepnczly.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tfmqjxln.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2djkkoifb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrexyncv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xugbnvsh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2enmuwbnt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dzijkwkk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gdlwfppn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2apvhhbso.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vsmlclqr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2digcdahj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kukfzrma.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdxpqnmu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2twiyfddk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oafxsdwn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2afyznzlv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wfafaylr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cmecskwh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ipficujk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ukysksxf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2puzhypph.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2udpalnum.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jklsvqqo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2feoblzmi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfjtqkkd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xejydlhe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2osyrsesf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gajxwpyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vmibfdut.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vrvelrba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lfouonfk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ekdlmgep.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lfudeeln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qekkcyjd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrkmlrxl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qlbvwqxl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2teyrhhtg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2avdpviek.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkddktyr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qkxbcikm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbrxteqz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2piuwiqjk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dugnjrge.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbefsaj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fyyxpags.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xvquwotp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uijhsrht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhveqotq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jslijepf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooakwkid.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ctvgvdqs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wvkazvfv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eabszdgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xznxpvgb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eyqemggu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2imtjnqyz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jrvxzmly.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ncqbqrgc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwoqski.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bokhptbd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fgqefbim.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rlpsumso.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxeszcq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxgpfqau.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfsxpxt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mqayywbj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hdqzygsj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2scopyzhr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwwemtua.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lkifnzig.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gemmhbny.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2agpirpoa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ufafgfeo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hzraqrph.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mixxwggs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2utrubsjj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mkwrrbgc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xqhyjylh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pqhtryxx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jwijqdvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rnzdqijl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2icmxqeip.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpbmmbzz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dsjxsasa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fvodqbwn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dsfzwlua.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gwdgmbcj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2khjjrpzq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ylhyaevf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sojgqrhf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jigubobv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2erktaewd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cisfdrkv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tlzmkpeg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wkcowhye.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yccvvefd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2periffts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2luupdmnb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2squktjlr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zchkmukk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2elmeclac.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bgrxmspq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ckdofkml.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdbraad.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rbdpaptm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2knpttlmr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twbhtvvj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ofatitur.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrcetqm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zopplbes.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqoihdgv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xknrnnas.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kxlaormt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mrsgmoyb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nrqalogo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vdsbikyo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uywwkdjj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2epxmlmkc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlnxihn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2piobcolp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fwauggdq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yqkiripz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2iqesorww.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxbqchn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bddfcjsy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jkwlmhtc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rvdmptid.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cvwmfluh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2grbhhecv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxomhlfd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2saikevys.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kkpgbfpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgbrvx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mufpewok.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ntrsavlq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mqmnotcd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2emutalbi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ipynjdcy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xoihiiiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yqmtlvfm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxwvabso.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cmlytivd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wlnejrie.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hciziihf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ioojadlf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tkdsnrnw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xqaqcjpf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oabtruae.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nkbatphj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qpwztllr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2needooed.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dyqhsbhh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvrpuobg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2govjnzws.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iijohuhh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vmdzsdub.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hxzwrdce.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gntozvdd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zqobeuzy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2voeeccgz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ksrjwfit.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wraqghfq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2prcuhila.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rjgrqilt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jkxykzoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uflwtlew.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjhjhazu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kffsenlk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2djfinssa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eiibzhat.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2msugqjbn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2spwgorcb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bclqprfz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cqpmuozk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rffsohbb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kpoyhmig.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2txrelmcf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsotvsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivrhecmp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hywvubsh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2uywhgdzc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2drvyejec.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qqlzhljn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eirpmlpi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flyoelvh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pcrgfujz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypioobsu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jdgehxze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ehzkthos.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gnptsxsp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qtttrkbt.html


<!-- 参考信息 -->