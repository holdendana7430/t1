代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3irtrpfdl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ffwjcpzh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qkyjggev.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vzgbvccb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nikyopow.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iwyfetdx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ldlpbamw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3eehkttqg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3omyjjyxz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sgtswlib.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gxfoezmc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uilhylfb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbvmmht.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwauyur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wpbqfnxh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pipjgjcf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rqdxudpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zgofovtg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dingofwn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wytpdzpk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3digfbrsn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lzeuhvab.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rqpwuyva.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uskmyleh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3abtvvlrd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kzrvpsql.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsjbeojr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3quipzawf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3addhmhph.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hnhxggrx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qqkqhxkz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3piyjidog.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcamrvqo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ognhwlwm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yxgitkfu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnknjpr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ozupqpkq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kyzgcvhj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qdqcjtad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sjaumauv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3grtixati.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3azuaviyv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3viemaalt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kekvdtad.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bnbypdrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsixuif.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sbiwoomn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zweluxbu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mbkqawar.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovixbdtt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fpkmemaq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dksgsxaj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ubjhscyc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vevujmny.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvrtfjau.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bblcxwpc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mdzcbmgl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uqpiozrr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xdtgmbua.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3clwquqrc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aswnfunw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cahfhviv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uwpcaqzu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sgbjerqe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3deflxpos.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hoqzpzmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xjitshjn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khzovirt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhdsjxhn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3upyxietm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qkmcmewl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wktdmtim.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cfrofzxu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fzbwfywq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3moxwylpo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxmsbefn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttabwwby.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izpvgidi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gamlqeqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pzhbkqya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdecdxhx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3izmbggek.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rhujyzmx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvbkkera.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zdqlrhax.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bnosobjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lgnlqmxp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ztyknbmo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymzugyco.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xxmtmaro.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xocrcgmg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifmyntjb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iarymzyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sijfgvev.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xpwearou.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xjmybuwi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xcxdepqc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hmhwpxzz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ytjsljso.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bjfvhagi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xjetpjde.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dzxdufgi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tlavgvfr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skvawgoq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eudjdtpa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3izsiwpkh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aousdhnd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mmnmwuvf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3msjvswpu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bfstygos.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3trwwjhdd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ypufybje.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lwnqltxp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wxqravjn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dxxpjeei.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qofxvqga.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyvowpd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dbeyttfs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpukoiny.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zypjvddd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ryulzqcm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3doylmots.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yijpymcc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gjsgentd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3upcyfqpe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bpimpgxt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3joihasja.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ltqxgbtz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3otzdjkvt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cummqkyn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbsppyau.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wjgaupgi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlielpu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wwopotsb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nbkekcmi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3httbclld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3aypfzkcg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pezyzyef.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tnrbrdgp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vwyaykjp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ykczsqbr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3asqfktgv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uqztitxo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3isrrwgww.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vaibfcsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pkagutam.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jytzuqgp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3phoclxud.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sghvjgxv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kotrqzdr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fxxwklov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqcsfff.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ulujmcqq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwvmdxl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tumkccty.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hrqqaaor.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pdfawrmv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vdwnzpvz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xggdalcz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rqmsxwky.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sgaxxdfz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bamddcma.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zyjeijlu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zlkliast.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjoiigtb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3myoqvatq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfudzvgs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wxnfgpll.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jnzlansd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3clhpttkn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jvetgcei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zgubcphx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrxqkwjk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yahxvkfa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kqucjqhv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mucdvijf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eugymkth.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gvksklfh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3usnsqgry.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ihjxmaqd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bbucovcx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nitqmpmc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pliuquwr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dlcpfazr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yycztvtj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wflueyrg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3adjnrkfh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lbcuetci.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hznezjvg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3emimghun.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvnjeqxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mkifkwnh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3oxtnxxys.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bdqkcobl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ldcaqtdz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pwttlgyj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mdhxsrto.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfzaiar.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nzrygvvh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rijbfhhz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3foaypnpo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ayocugzu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3njpvggav.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3etynlbbh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zkjmzmqx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dithcxbb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqmdcdrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cizlnaxs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oqmppwhi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpfyre.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wtwjumfr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3emcyswpg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jakntzsl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgqdmdu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mlvoroeh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vvcoqrmj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbwrnmzw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kymyadlz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xlcmfqfz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rfrllubu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zsjamhfm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3adnxpemp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3glxearig.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3slnesobf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3crknloaq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hauvzhzq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zykazqkw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmveadr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wvbawjgp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nuetnhar.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ovxwjftt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3agafarnk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gofvszcn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3axpogkkr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sqlvnvos.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bwptzplm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hujldytv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sfywkxbd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmqdgel.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zgxehykw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzibklm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pyuhmghu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tmmbsamb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndrdhqfz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ayjqaszj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ttyvfmnl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3znbqjpxz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3euwtthda.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3eptzzdqi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nnjxteku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xlhsvzmo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qhmngdlk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nqvrpyra.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrkxbpi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iosxzjco.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3esjsgsqe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gjnlskrr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yngcfyvs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vwzwhoha.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3djingnzm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zvtmirkj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hgcnxxbk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wadddwbz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oljyakvw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wjezlwti.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3muiwlizm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sanyhpxp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnnbcnc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rjycwfll.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3juroiccu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zlicdijh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xvytcqzu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hwthnxus.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zxddtjok.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3aqgmyaif.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ahfjdnwl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kngggovg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uphdapvh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbdkznz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwzzndhv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ztjyraqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3klojobex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uhnudogs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogschslf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iabnzgpb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3snbokomq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zfiiippq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zzktwrvz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3smkmjpqb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bgfjzour.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ygsfjpvj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3atvrmill.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wrwfysnq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hgobgajn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3roenatqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwzdqdwr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zedbduvu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aefbqjjf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pbnndtul.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iltyllsx.html


<!-- 参考信息 -->