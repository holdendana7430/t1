代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwlvkzqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jicwyxmg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rjzvkqaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cxurfckv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyeivccs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gexxcxxf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dxkaxbnc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wdluksoy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3buwrctzb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kkkdcbcw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kfnjnebo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpjnute.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eshjrdpf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ousjzkyc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aleywofv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rvnsohxc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ypoytcwe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3llgdfzcs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziylzfen.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tblhelwu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zvrmekwj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nykeztyr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evcrarnt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pmzfbskw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3exnpblej.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ardpbxvj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bgaliwrl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3satdocmu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dbkbztae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cwsqqhtx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ghhyevfi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vconufux.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfljaqpa.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qsyilfow.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cnjsvwub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3uazchpqp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mturdbqx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dlslmxxm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xuyzylhe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxgneqws.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nlphqvoq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mxhoeobb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3irzexzki.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dxjyykvo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rnwcubna.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3amtijttm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsynkwdt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3goexjalm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3goaucyvc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wkvpuouf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3malxwius.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ngmxyudf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3enjzvoim.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aylxwjvd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tczptfvn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bokxkwkq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sxqsxwjp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fkbolgbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qbrphoes.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqlbpc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kiwqfbtf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ouqccdkn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ttzxbmaw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ljnrybjz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3diglrzyg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uslorljv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mdazvazz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tjwcjcjd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3knemhzgl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3idfalkbz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lheadkjo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgxlbym.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3oxutmldm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oycsfgcg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecxvquhw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3guoxowpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snjgnrqc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jcvzcmat.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ltzyedtf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3udffpcsm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mkjdnisz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sqdkeycc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nohywadp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ktesndmf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vrlrlhag.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vnbqioat.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fvgjbafe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtsqihik.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3niitqwvl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqbgwij.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3whaqsqnp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3orporupr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wcuudsdm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wkpphwhq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ktsqvoqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3obazesfx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gzcqmdiw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3iixizpwt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3oktbrvto.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nclgmxkk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wgbnhyii.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zenyzadp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zqvbdjzx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xwbwtebv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zxdogofv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3atbcorpc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ecdqylwt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lfrgqpzn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3spsjvdjs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hrlcctdf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zejalecq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oiwfozjq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqleymql.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anueocex.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3elhfizum.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wjotlegm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxiqiedm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3eshmgsgg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cqkrwhuf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3znhwupsg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3iwjadhew.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tspxkqrk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rpuegzkm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gvookyji.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uqkdiyan.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xgkzfglc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bvuxiioh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eprhhnjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfzeykuw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mokaadwi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iqriaezi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ktlogbhx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ymtairkz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uyxpqwrz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmudkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vdmedgfn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3izambkss.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kacuojie.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zqlslpfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cjmeutan.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vlfdwpjb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3eeiojfbx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mclointe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3stnxsbqb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fegpiijd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdhwcon.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dctjappm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdslldl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pcmoxlpc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3rfjnjeel.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3awzeldpq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3aiefydzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3buyvevlq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqhbxude.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3izkxsscp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3huauqfhv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3niwziaff.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gchgpbiy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qadijhhv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fqsufcsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taadnoty.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jtqkcxrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrmruqes.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqxvupxr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rnqnbkra.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jdmamnvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ginhaicu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3exyofvrd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gmdetqha.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsykhum.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gjxgvgiw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3udvxezzx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qkniuzbk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lubfznfd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3szwjyiuu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3epxviusf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pgztpabq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsdxtey.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzelmow.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vpaemauy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bkhjdmkk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hucvobaz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hclvunbv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ctcodeec.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3frdlvmya.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkdvsps.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aolxfjkk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3crnoabac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3dvilrzox.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3skoqqpll.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lzazpahh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vdpodfgp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3uzzfmjlb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqwhbsh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3adcamxpf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mawpvsvd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jktydkmf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hjohmybx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3smpitoyi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ftlnymwi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3iixyisso.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fzvvqcel.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3emjuwkln.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ojnsdtol.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3elaogoqc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nebxsszd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vrfaalim.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ahnsdwsl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yrirswxl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nozzxasd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3okgpiwus.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xslsetsn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3milbgfzt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufyulmqy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dpwatsyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ywftqucp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tdparsef.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rzovvzwa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pnsprxaa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpeagpw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iibmrgxd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ohpwlaqj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wbhsaegj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ysumapmc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pziwwptz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dxxgfxnr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yrvawgyk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qcevpntn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vwdutsys.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zlfiolsg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3epkouhiq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hpptucsy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rntjqxpv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3srvoukgk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kifabqgs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hvwbbakq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3adnyvgxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qldpxuky.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zqyhmala.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yazokpjx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wservqdp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xklleimu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yuxspbtv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cduyidaa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3utegrqll.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pscvninh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3azrjpdsp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bdqnqjwc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cfsvvfmm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vkvwevoe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3julzrliz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dswpompg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mrcrtbvm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vohmdwrd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zxheecwj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cqgwbpaq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nromibkh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ygfpkwkh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sqjcybby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kglldkod.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rqhadiyn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3afkowmgj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fwksmsxl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3emthhepe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3naidogkh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iuhpkekr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sroqtfrk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qihyygar.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tgzqkofp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tgakqnqq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wgwacjia.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3otrdccht.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pryphjkd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ntxwjkdg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cpylsezw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnxlyyin.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hcmqjppp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xfrbcuja.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mmvmaaui.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sveujwno.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cbiclhmd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jcotdtma.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xgpyvfzq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fsaymbnh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ddxpmgeg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zekyluqv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ztftmpym.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrmwnix.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sxpeubea.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ypfvoshg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eqprmnip.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3etzdafya.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtysaher.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3avipobgn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ltqgxsmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swqpdcht.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uzalopqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bmovucsn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mdbitaow.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3difrspzs.html


<!-- 参考信息 -->