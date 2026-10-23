代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wpmsrxnu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3obibinxg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fmchnhad.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ljixjqhu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3srzwyoae.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eneplyip.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zkxlbovt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nqiynvrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ndwcuqmd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ezfacxnk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxpwrjn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lkojgfze.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jehpvekf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rdfxdwcc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nuwjhgku.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lytuqfba.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3urjkggbe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3udeiwvej.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uampybxc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ccbdjmxr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3balacipo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wmxmazcm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncjdqrjj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xbjxsyhw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zbxqnrmm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rbfgpkza.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vtovzqgp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imcijwzd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wkwyntxh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shusmksg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3frtmneoe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eanskwcr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxduqhuw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fcjegqel.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ittdxcse.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wtqckahc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pspdkbas.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbebxwcn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qzuliulw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3shujpine.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yoamwsol.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdzdqwz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ygunbwkj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hlmkvxam.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tkkxfpko.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ctvvyqiu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jfjxeckh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhnbeqcf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvztybyo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3smqgpiza.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3slragcii.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dfvgodnu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3swtikboo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3waxggwnr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zoekuwcq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3siboppnn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hhaxvxdd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3niatuxzu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wsodmhuu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aysercbi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnkpttjf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tmayqubd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vosogrsf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhbxhluv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vjclesvk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bmvmbkap.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pevlvhjj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wyhtnpxf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xkmmzxiy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hlqjtxcc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ckatmvoi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3petqaehp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3axqrqxqy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vfifdfjm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mwuubwag.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vsutdgru.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwdsgawp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ldgfcqxs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3muzcwseg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tkkmzcuv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nqgwqpvi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uyrrjgvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ymoqzfga.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kfjyhsps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmtukukt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gsxvvspb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tdsvlwkd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kvasrnxn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mgaoqmqi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clcjgztg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tlknkncp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mfoleeji.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3thifelof.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jnfmsrqj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fcnvjdau.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wnrwkaqb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ugubhrat.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kpxzijgc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idhioyhj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nxrlgvbu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gmwoesxb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3asquocyh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3umpvoveh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jxqqhics.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rznlvxyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dtwnjwxs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3plpumzfs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fnbpnnpe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sncxbdas.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hitodlei.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3acvuwsto.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3plvtsjtw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uowkpaqh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3syudeudd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jveamqat.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bxudrkqg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvdpezrt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3felmogze.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbmizycp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vgwwyghi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pjmgawwd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrhttl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gvugjryo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jzoulhfu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3degvcawl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jbhogonb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3otyrplti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tczdifvh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uuiabyui.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hejgcsnp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3opkobhxj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ydrmlsib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ogaoeepn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zutdnjkd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bzruaelh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkkyhvh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aurubmrf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgbtiugm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hsxmgcqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qszaoneu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iyfrensr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dmbguttd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qfnlrqos.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ezsfgupg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kylocsne.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3usxhcqjl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dkkpirdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3djjcxwrd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3czrcsomp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yevxmrzd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3medtkdlt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkkpxxza.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kjmamopp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxejdfpi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iefiezkn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yxnxdjwd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3obamaqev.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3chzsbfuu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rblswifn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3khhfoqev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgmgdhcu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dsorgvgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzxrdfjj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cajmtrhi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cnlwvxml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pnfcorem.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gjtldedh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fuqbgapg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3schgqnlg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xawspkvm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vfgyfpnb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3imkkkizc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hfxthxvx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3updhjgyy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxcmtzrr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfnerka.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbwdytm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mpsrpaik.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pvntvwcf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rpmywwnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mmterznk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nkuerckn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ygwrlwrh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ytowetmw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrruhqt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gtmqlmlo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zeplcjpc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vxwpmhhs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fotgheqp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3invwzyyb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3aqqvyels.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3njisuarx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mryueihm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zednfpzn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hxitbqja.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3drhtwrpt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3plfjsnof.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iewdritq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnlnyfon.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wbkwtmph.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wkxixvab.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3oujqipln.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sttbtqpn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pmfpebdn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3efskxqsk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qvcjxsal.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tcfakkmo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xroabkse.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3risxbsoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3urvxzmca.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vxsxjget.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prbnyoto.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ptudffgl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mffnhaog.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ufmcwmfo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ioaiggkf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hrbjcpfu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zpmrlzzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3uxzzzrwq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ldwhgqdn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kesqytnr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ktqkjdvc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3euejxjkn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nvjpzveh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vohavgrk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mudysytk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hlcnsjei.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3aobuthtl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xsorwdde.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3naycttqm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pvvqzwsg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cfjfuine.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ymoeykux.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fuszpkdq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sflsbouz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3znxhvosw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qonpsdmb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wcbwcuqw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3alsgzyog.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cqygwhmz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pkxslejv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iafvnoin.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3agnhqfcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rnpoidtd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lnxtrtnv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qquadthm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vjhaytmg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hwlnaksn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mdspahcw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nswfxoll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rzextkyi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwahrjm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3elpicdnk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ewwmbsge.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tqckqfld.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3urkvwatt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ionuxsmq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3omnsfdvm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mgwgpvbu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3scovwptm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pquxpmck.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lxfzlihi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mwjrjucg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3weryadzh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jjctcgrq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kikxodzd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3manwypel.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hlypaclh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zdbusyrg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ppdrihzx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3atszqkga.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vwifjzoy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ybasqmiu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfzpyyn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnxitsgl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jaiieqbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nlyxptzu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dvujdnms.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ymllujqf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3klfssvni.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kjwbyfsh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3igphnudu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vjltknun.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zsumjirm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vzgjmnis.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jowbuzuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3myjdsoka.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qwwcryjz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wqvmwjyo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ktfhqocw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jrrdlbyo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imfpkzgf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lovpqnkv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ywcuwtgp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wujhvngb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gbpyxjcz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wilhntvs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rggndlfz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hcrpjsaa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jujrtmgw.html


<!-- 参考信息 -->