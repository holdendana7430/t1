代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vtboynml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jdeoggsu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rmpxweda.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2siidlqtu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dpnowbbf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fwbrjbyi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2woiacyyx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2efatxows.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dyygfpzd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fxrvbzmv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fgoczecg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hwjhzugs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2osjjqkil.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2eksdzszo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtoerykc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mfeygefw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nlcdfoxd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wxatmmil.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mqjuhkov.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbthrjfn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjujrjxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tumlvoxz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2odefonhl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bezypqth.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gwdlroct.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jfqewfey.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ebnqcgpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2eeesxlds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hantrqex.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2msofxmfg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brjbjgmx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjtmkink.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jrviqoah.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sllaenza.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvqfdaig.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tuztkwui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2atjecbli.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2moaezirj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qhgpdefh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kgjleccl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsiklnis.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2utzxbfoo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nejuumsm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nriffmxm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wqhbuhpp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ibypgirl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2akfrukpi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2scnpfxov.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wmgjefkx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kelsvsed.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uwlywvmm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qtikkksm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwuieafr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ffwpevsi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymioyvqa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzhaatot.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vtoyhnhd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nldnqzrf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2izzdxphb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fbdwsijt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uqjgxywg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2feagdpau.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jzjcdonc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lamzaqsi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhwebnib.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gfwszsmc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jeohbhbk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vyewtjcs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cxugfsip.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bkavdfox.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mryzuvkw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2cobwtxje.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vrwkiqcs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2banrmalh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jilgrvdi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nusixfyv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxdgmomf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdugpbpu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pyezkvcl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qjxqyaqj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lzdynayr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvolhli.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tyluvdow.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rqjsonks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qccswxhi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xsyecmrb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2udiwgfdk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmdbjdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zwulreje.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lppamnie.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2prriqzdf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qdbpwfqk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2euuyynul.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qcbsdnjf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2kdbkphwf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2axdjqpwc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xovjuszk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xezeglds.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2stoizupi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nvuhqcbf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bymndyno.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ipzbgapw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccifvqgv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmvnxxxn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rvztnmwb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmxtvty.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ligpqbkg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2puzrnjnh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2prudhoqa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uhwhwavx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hltjbljx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rmnkoupw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dtfyxqyb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2drnzkbzd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vfoxzrll.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ggfdmddg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ottildeu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfppscq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sriabhel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmkfpejz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xandogkl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2blfdsubq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2llbxwqzh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uunrsxep.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jnwkleep.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2koakvrmm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zjpzksla.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ccgedeno.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uijtbgfn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sovupibq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pizkfxrn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2emprhayy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2czoamwyc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nxqggrga.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gsfojdhb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ziyvyopj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kdimtphf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ukxalmub.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2amukmdlw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srsgzvqo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sewlclbk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pflpdlnn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrnsawhg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pifbukmj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pbmcjwou.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bmqzyrfw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pyynuqei.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jglvmleb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mzeecaqs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gvfdgryr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdhfhro.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nbmctmra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glmrosjo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tcythaww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkfpmzbr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tortsljf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bsybfoji.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2purwjdhj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aeuhuoos.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsymdpt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zlxmlqpp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yrlzhtyx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ovdwrcsv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2govqhjhb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkamkhpm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vanwrnly.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tndiuxkv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlvmldd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzokidgq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cshchakg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2atvzpcla.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rhacfjir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uibnvzdw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2recegevg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2muikkfgd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xdlvsrvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aunjlfte.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oqzgpglm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sqwgmtqj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kaminuir.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nlgbmcfd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bmczhsig.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sekaisui.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kxdgfubs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fkcrilkt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzcjuae.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fdfwctds.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fhphajhl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2aezetsae.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajlevkdm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hzetgljw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2drefwjjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ksvjlzqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2uzlqmeyg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xbpumoqf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xdalsiwz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2irzsydfp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2snshokek.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2axptoygd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2puibatee.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2myhqcgym.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jhoalnmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hukrjcuh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vxcmkmqu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hswuyulp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kybjkolz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhghrqh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nxvmkoso.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixksqnqh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ploixqbb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uhvkwozr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2diodfwqf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdofera.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lllnbsww.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2emewipwp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cuzsbthq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2nbaezezb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bddrkgzu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ppccslec.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2eryxzyzq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sfnbqftv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2seaslhup.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bpvakxtc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqgqmgh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gvuprguw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2btcswquv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nxtafbmj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2uqimxocg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2abgxwsbx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bnkfpryx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eihhygae.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lfabajfm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hdqnupzd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfcpjha.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxetgadv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ppvtsamj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2btugngsk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2atgjnzkz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fxhmpjed.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ivkungva.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pesurjpm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ichbgchk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xondqhcz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fnstackh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2elatdvci.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymgetrso.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2excmmreo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wdprtooy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ihcucfmq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvslrgv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gxpqsagr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ukfrfwhq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cuhzwxee.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dgbvjibs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uekuzkeo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2obrhubcn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mfgttdii.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gkwqccsc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2juzzezgh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2grqxmzyg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ykvhpajr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2awlelirf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ofsvqrmg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vjnvjsre.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2frykmsqw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dnwiftjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkpnhyzw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yvecdcsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rufyzsaf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zmjrbdoo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ahlfzwoa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2anepykoa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sippwtmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2azkkabkl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jdlyewkh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjrryjn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qgrnxdct.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ujcsmafc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fdjauwwf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ifevpeks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wvjelpdd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bamlxgbx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pvimymvx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awpfqbvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mskbqwbq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2osobwize.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yhfcxtuh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tszuykzh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2izoundpt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufltddsf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pnnmyxbi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wndyglwy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2oiraofbo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hbslrekh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fwwnqxee.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oslryfpk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xvrmucft.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xteuuhmf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2heenorbx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2utsfbxab.html


<!-- 参考信息 -->