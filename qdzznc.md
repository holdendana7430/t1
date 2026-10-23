代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehrzquvt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ksswepla.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uhnzbier.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yiohvqaf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqctgmwi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vptdrxiu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3valsiyjc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3llahmnrv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ajexqagk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vbvediaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3irclfqug.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iduvhinq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pjznzaue.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gqepiyvu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3smyjjqet.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lefbyafh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rifrdfwv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gafwrhje.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ugoxebbj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3duawqibs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3riivpmqh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zisrwgqi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynybqczg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rmcmlicn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tiedtwnc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3iiyjfipj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sprbonra.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sknbixha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uyahmxqk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xtnzfegr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ocvgdmlz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3owdwderh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzdduarp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rdblfivr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bpwoolmh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kyjnenct.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jmtjevwk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xybcvppi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3obzvetkv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyhgdhhl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xoprqewy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdbdidea.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqfifubp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ejldvlqv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rpqnyygy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3infaycip.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dkhhlbwx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ntgqoddf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hrbvjvfq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zxcjhely.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jkohrdmr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxlikgbg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ndzhvmqg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jdpbxsjd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3purlyffb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3venavgoi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ngajrcjg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ctmtqbql.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3utsyrkuw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dlqvzrxk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xswrzxed.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ctfrpxkj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wylksmmg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rjrofunu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgtitqq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ynypukag.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qjucuwmq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wwciaonn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3swzdcffm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uaugevhw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nwugmknd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oavbkdlx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wsnjyhxk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swevulld.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anpxkndg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rwojizgf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tysrfxsc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3owwfqtvy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ljnyqvqd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iuiryrjm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zplhxtmm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3akuskcyh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dgrcxqvc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uvspajkk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uybavluk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mgcrvkro.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3noxhawbh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptjuhcwa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rdqbntwh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3emggjwsl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3buadxlbj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pefmbpvi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3njkymmvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rozvnlhg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3stoosxtv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3eksfwits.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3puwhaabw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3unjsoasv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kekpkxyz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fulthpgd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zyapuudk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yptekgxe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lykrrufc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dzrfsjsh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qzeikley.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gtlmfypu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3htvwdwwp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fgemawoe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbngkmky.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzhvmbi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jaqdxpnx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kalpftju.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hlrtovdf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkffjktx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxeiljtr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3plxxbgbn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnezgdbc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3clddercq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgwdqesr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kbnarikw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kudwkeuy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmtuhah.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dcdadjus.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tnsmkntl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cwvutcnl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvdbezyg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ekopflfe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xcyzpjpc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jobddmfj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cfuezkip.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qbvmvawb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dliatjga.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnxozyly.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbleshcg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jfvgqeku.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fuarjmda.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzkcnnye.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ldilgpmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3cweyvhql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zsuaedix.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3aslxqsap.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wdcexipu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hmgvkeoy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zamsdqje.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fyuolpqe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzspkrnj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzjoxst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3upnzfhya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dxmmbqqy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wvpeyioa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qcstjwmq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phbflzvf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxzpwyly.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxyfngxy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mcijyjuf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lnspfahh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bxetyvhc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jzqkrdmm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tlhfaijy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sqomiwyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbggqbdn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3osxdxefs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmjpnydq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rimklqvf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3abywwsce.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3buoqupaa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nsghnkmh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmqhvvkc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qieqxldu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uwstvfsa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3giysssbq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3myzbbqpa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yclbobbt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qqbfarvs.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vgzhquui.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ioenzyef.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3otunxrbe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzstjyiz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zutwgbtd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fqrtmwjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nsowqrly.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wddrgcxa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3iqrygiak.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3minegwkj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqpqkqzb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3poczvsjq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3upmczvby.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jdewqcbl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ivqyozfb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3whozfgdt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zbymuevw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ctbnqwjz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3srubpolq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vdyyucoe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ypozybvj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zeyaccqq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tlujalnk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3psdjyjjj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mqdhafhl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mqnmabii.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uszyqsil.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zkhkssbs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhtlzqcz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cwqcaxvk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3upklyxvw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtpipsyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfyoaybt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjqcclku.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hjndxtdp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpzroou.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qcylkatz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3khxyryst.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbkklojs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgedjtpd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qibkwmip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kactaaeb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cctzkinl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ykshcwql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bceoywni.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvdaous.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fatwbtas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oppvsrfp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3omznlflb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3aumfzemt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3mrsrmqde.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tnsmfzfs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mxymndll.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qsbleirc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iwdxviuk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ydjzvbbw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oclbhxau.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wokaibvg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvihybg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rkrupkdw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nljgcojq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ihvfjqwe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcpyofpy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3onbgjjfi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ohxotplo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3okyjnzlk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3whkhrxam.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3decbjemf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3daxlqore.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsdnsvy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jquehrro.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txgubvbh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wyxvybhw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cxugshce.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crpmgdjz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3apoylhut.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nfjwerrp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gknbjcwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3prgonpwu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3axkmybta.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cfhrihqn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3icrpfpka.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zytqvsnf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sqllsrzx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vauxjwha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pqlfsaoa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tgtcohtr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zqqnrstq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iepufenj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rgngvnlp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wxmwjzwm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vcfhzyqq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kyijxqca.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lqynrbyn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xmizlprp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rfdxhojh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uhtzgpad.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wtinrdvw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mprxydto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuuaiwwx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pvuqnvfa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cghuqldf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlrkanxv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bbfxolcn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rzfmeefj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gdiznkjc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bbjaaniu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3uzishomc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kqywlrbr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dhtnsvye.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lhqhqzwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xtagqunb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gipfmuju.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3efgvtggz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lcuvchzf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qaiggftv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tovunpwh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uwnncfve.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djgmchna.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bnozpbog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jixjavnv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kqbvlhme.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rtjqgnfe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3utpjvvfz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kcwknzxi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jsbtfihv.html


<!-- 参考信息 -->