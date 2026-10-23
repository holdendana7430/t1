代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fdkmffur.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3unjqkwcn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3agavbrcx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3homlezio.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vfablxve.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vmkpbjjd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jjohjnxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jgpzpkji.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iznblnyw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3retqnjbd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hqvdfkon.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wpxgpixw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kazjcwph.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tlyclmje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dusfmllq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mfdcvead.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hbrrcqux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ardhnfpn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nzhuznxr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yipsetix.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dtaozzfn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3apcumtac.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xehcdzhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vlsduvxj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qmbzbdwu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vuljpjev.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjmvhsm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uxbybonv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tgdkngem.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qfaagaha.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kssevlmj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3refqolvj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wbsgvsyh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyyqnkqi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bhlolchu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozgilxcs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dpmpspzg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3brzaoeyo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mzzrvkax.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3medkkdzq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rvklbykx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dbwpamre.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wxsnqgap.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqsfmitg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zwxbpwjd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uvsomhtb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yxmgwfoa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xaypztrg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3eepxruxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hncqfiom.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lydqniyx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ccidwgum.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gptyqnyj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qqiqzcfm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rnlklmat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3crunqqns.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ksuslgkl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bagfmciu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xpuprrjj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qnvczzcz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gcjgpfmg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rvffpljj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hfbcoxna.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3knumyilb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zisfyklw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ajuaurto.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rugnsrdc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ayvzskgm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzbfmyi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3znrftkrm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ntsxlfjr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bxdrscfe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xchizpif.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lcrmrnqf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3glqcqwvx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrkbouyd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3maejgbnt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3honaxhqb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aiqasqgn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qxuxchnw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwztswtk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qmdikfvd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nthtqqvq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nvymdrfd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pbzbvapw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ovlntexm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xylmguxk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jcidfgul.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hputkdqz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxnfyakz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hixpzaiu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxliowmp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iqewmlyt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wswxfzgq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ggxptucm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tflopkgt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kwujcwiq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nbecople.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lxgbxhla.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3teptcoyk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jmfvqnmh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tkotfnsr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkodpi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wahpweju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3usvdsyoy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ltthlust.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3iszttqay.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3valyjcqs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yowadwzu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3egxtpyco.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wvczyizt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jmreadon.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3coxwrisn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kkrptggv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jhmxbcrj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zyxwrube.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ihcdedpa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ricwttuo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmunfcoa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hjzgighy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbfqpsjq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nsskrcog.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgjdvue.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fhaqnypg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3uwrxxwtj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3erzmuhsm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fqaqyzfn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3osdsimlj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gbyyeuhs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxokkbb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uykokuxi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cetlwqmj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmswdbab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3oofhsdro.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yplntzgi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cjnsnjqo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nitaoemp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ffbqunro.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3napxnxes.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3njdfvxgp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zxpgzdst.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hyntgdvc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ycbiukwa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3idinomqi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dcdojvyu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sjoqkqgg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rgtmejit.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gkknmbgy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bkdqanrj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxusnis.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cbowgyfp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eekgetme.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3witbkwsb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlgnwhj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ayhzlakh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3plezmpee.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eagnvjta.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bwefzbla.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zszgdijz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tcagwecp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ijunqzsx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3veuucqnw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gpiodyiy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgjevxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpmoqfyj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lcdrlktp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdrqirdo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3haxunnfx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bpivnqzo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otgkwbxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iosadhau.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqzurch.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oyhfrpqs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jdslwpke.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yqnfeomq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nsjvdbmp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdwbymey.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mcnawtkn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qyigqplw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lunoxekl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pescwgwi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3senfptoi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3shvlfktp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3otsubskb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lpvhmbbj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jtojasxj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3icwkxwnl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tziguzmn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ezkgzfnm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkvjjdg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fzkrlsio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3otrjpklh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xxsieswc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xwavpazd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mkjaeawp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3muymtmew.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hovjzype.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ncquesbl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqfhpxut.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ibwfhadu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3umxjbzkl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3keqzpqjk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztbywtde.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kfajniuj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kpdnmlxv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tetsuzvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rsoiimyg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3socggywx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pxcrdiqq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnamoeb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dmfuftrp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mfdbbtbf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hkujsres.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bvyxckdg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rlhpolek.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmbpabot.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3isklklup.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wbdnituh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnwiqcc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hljxoghk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3txszshqo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3syqbjsmw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dmqemzvv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zihfgwgm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqglpqg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hmwllldo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xoasoutr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcuyzvmy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3akfsrzxr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gcidlpzs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrqggo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3siybfnxu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3japjnobf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pbawlrkr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hykwmgxn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvcebnb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cdodlbrx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yjkuznag.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qfhetvxl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3btizqais.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iulgzrti.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tuupuhii.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mnwmovvz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfwrlluy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aywgwigp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uhofydbb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jrojjbga.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cywwzcjm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dftigrte.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zepwubdt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nwovucwi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qdaerzie.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3skeddhzc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxbfnrq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kvthzebw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3muxdniwo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zduptgil.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fthonaxo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3etrwsgis.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdealelr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hxnemccp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtjjfixg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3unkrxnhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3shxrsxxt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltjlyoph.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nobaspil.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3omjfkkdu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cuiyvxfu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gkienocc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hbbmaugk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kckhtbsh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3idrldbza.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vyhtelko.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qsacqvis.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ywaikmuy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lkmdaunw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lmsztoun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ashncwpd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3avorjrue.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tdhcuzca.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3smtvbsne.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bqpiuopr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ozwjdazo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zotdiypx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zaocjbcd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qsmlmjoc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jsyrwzqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3aiidoqet.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqphregz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xotwqfmz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qqgaayqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gcodrmce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pizwgxgt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dkskdrya.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hathgyax.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqwmilkl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nprduxul.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vbnbephm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lekrrqpj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qayhmosi.html


<!-- 参考信息 -->