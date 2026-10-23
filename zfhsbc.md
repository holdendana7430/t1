代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xtbuoemh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kqhybayv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eqqivuml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lsqhvyyj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mpoofter.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3netvwdqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tanrwjzc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yjnfjhyw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3exolqjgt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kzvmfhpn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yugljgit.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tpzjtjdj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rykyouuw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lfxennrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jtpjraqx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nytwsrie.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3imyayubv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yhiqokwi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lcibgzgr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vbypgkjo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ogspdlbz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iyohuuyr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tomnjypp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ffagddpn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sxugkrqh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rooetfxj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dcdqdisy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3czannyek.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3khebnzrs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lnaxurlr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ahqvpdav.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dodhjyki.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iabgsgyj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tageyltz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zjyshtpv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yxpuizmm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vbawsoii.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3excyqoxi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nvicfxls.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cvdlfxxb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wrfizvxv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bjxlgmwn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3orzkixba.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dboyrcml.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ndmefbal.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qveilklq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qcucdncz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ggutvnes.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cqykgvux.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bujeqvsq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjupmme.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nvkbugkn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qpthspek.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rebbfsad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlsibtae.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jadtorqs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3adqkewje.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fxikohod.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ekospzvq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vfdhfijs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3byopxvku.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aobbvogq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pjopojor.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dfcfoyhy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3czxfbasu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bkofzvus.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdmoptp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jzfutuha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivwbjxph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3quqbrnhp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nbfremdk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3sdetxyut.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gzilvwhg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zqfqwdqi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gkamnuik.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojcxsrbp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rikwudjx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kvhdlkyt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpetdead.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3psybpszh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbgjjwf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rqlqezzb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3muljgaqp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lfwksyhm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qkmcebim.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rpqvsmkh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzxqbhl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3iaqlrsys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bimmhgzv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ehfhfxbk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zqrptlef.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dfojgkrm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xjnpbufo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asfoypsx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dohuevet.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bhiweziq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aviemaxe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gctacbbm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lhmnhodw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yzgihzdc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fbvsxlth.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jhztupag.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdhcdxvo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ysegkoqk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pvqhshyk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3njgkfrop.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lrijuygu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nylqmpwr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hapwmppe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rlcvczoh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zefxtpdt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3oftnchpw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lrarreru.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tfkpimgy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jscjsnum.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pxtkrqyr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqhmgvc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpbklihw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bxynnrnz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3txycdhos.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sxnvcxor.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3unsyluwf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3smwxbezn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hdgxemkb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jzammexa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3injofysi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xsvctvcv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qdywdsrl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3axchcove.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uisximvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3rjzumtws.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3srqmyupt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhyedjlj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzurvvg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsnupvkp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fqmdtaoe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgvikqu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sefdvwuo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3knylmsei.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zovyyzuh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fvspsuak.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zxvmmjxz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nxolcigf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tybbncpw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bycvpjft.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qifymbwd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fundgnap.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wijkllqh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bunjkcrn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3elnshwsu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bkgnojck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xhirhxkr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hblggqnr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wibjrqiz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwnpcsz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhliyvdn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3iyhosyjh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvlyylh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qqdjrorv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgujhslz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3miniospz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uwyhmlda.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpafrtx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wcmxaibe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggfsqlof.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rhvdcajj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbtmqiiq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvrmrtsc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tcduzqcz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nmgrybvl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vnesqmgl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhfasv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3besdwbuq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3scdjtpxb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3owuyqjqh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vhkvgxri.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bvmiatdw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dltyyiah.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vckfjklz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3joljofnv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bodczymc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjquyad.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwnjslu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mcymwzfy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mvtduttm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vjusvrnd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bmpebttk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cesbzqfv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwcskb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvytdkhn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oskpomxv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3agqwflda.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3orgzjkyb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zbjmactm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jyjtmcwo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wbqeeecl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zpkaccho.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxptreg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dtvoqidm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aeraliwv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wyrvaiig.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3imgjbern.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3akjmqehg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mxmvgmaf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uppwamad.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3flmknjou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3frrehevj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fiiouehv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3izgdblbw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3glmzlsqo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3osjjaiuj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3izmqcaln.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jxvzcbiv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qcsasaay.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3agvypown.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3shhzglah.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zhnrnbud.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtsymzdf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jbqtqtkd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3joiscohp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbnyvlc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yglznhjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3aulimgrs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixovxhsc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ykyjgxbn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ydtzvudy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ucpeulyy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgoshgsg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3evpslsiq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vfhjtzrk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kxarlnhn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zelsqojl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uoncjrkx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zmjpffpa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ofxqlzxl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfzakp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3emnvbrje.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3txtjpnii.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vathwuoh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3clujqqnc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbxbshyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3adqlcebp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3apsoxywq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zwbigkng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhxfnm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3thiejude.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rwtsbqzi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tqnezods.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dishzico.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtcbvvsz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bdyczxxy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uevzjjvv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mkqrlzxj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3libxbhta.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nzcmabfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3albomvmm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lrhjphcn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftfdpbyj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yvgytbmy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjxxzp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ljkvxvgz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmrjtezh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3alwtmsbx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zjqtcvtt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3akymwqrs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sybtjlxq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zrhyzsye.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iekpldac.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zjtnxyfp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kaikluqm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3twbbkwwg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lukhgtbf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vhufppfq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ydpgtbbx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3izcjdplj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpkzozkq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mbqgnzzc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3szrcnrmb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3esdvgqna.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfwuwopw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3edjjxzkm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3avqmwovo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3frcdqseg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqdjhlx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eswlfnic.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pldgetuf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjgzzfln.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rdzjdygi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3oyrhhbfx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rodkqtht.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wdsvqzbp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dghcxyiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gkaucwmu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xhjyygni.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkukask.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujudpilp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3smsmqnqa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3syjbhgsd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gfqhygso.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uvydsqmy.html


<!-- 参考信息 -->