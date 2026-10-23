代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mxesqntg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qexeieym.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxdbczza.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rhscawsd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jhspprye.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfgzkgag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ywhhljvw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ffftqgxs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kzntrdbi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vstoghbn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3thzkzuhp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3beculaup.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zoujhsgg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pziijiwz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3oxjuybzk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rdqdfpqy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iiaguoga.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jokpcyns.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ppkuseik.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zigywxqy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rlyeqhfq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3znlgnbrx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzbusxr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zotmmepw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wrjgnjuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gxoycfjw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oofpvgef.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3migkpmvc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wcwgrnzm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwcaxgy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3carcrbhq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kdakswgf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hajyyacs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dvqnzjog.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wjxdfwuz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lockgtkt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kiyvqhbc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3isalcgvt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ilggaint.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dasitlbe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqgvqrmf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgngnr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ttqsvtuj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gisvreth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtbccmml.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxxxmfz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3idnnrgpf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ehhdvynn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3popjssyv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tsosftfc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cydistfp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3svvmqxco.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ipavzagj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rswofklv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhmfxwt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yieylpwn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lmvojomk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mpvnbbow.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ceuaxrvq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xeurrdbk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lozwrwbk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wtpsfpce.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdbxpzm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xqumemkh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cayvyuez.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xoqicwyz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zunqfxic.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ltsmzbux.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wxmxmheq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gdrpqdfu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oatyukop.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ncwchvxh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cvyfykdm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pxhfrukx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hvspelug.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3druqmopw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aehyrcrw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tlrblrpg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mdusnihw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iznarfna.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pbjyhymn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exmzxuqb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gleyezyg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ajcpqvjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dteskwkc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ieqonsti.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wqunhgdg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3elanukfu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ptduuqct.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tfxlhenx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oiafkpcs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ohsvdtno.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrnurmpz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kxvqjauz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lcnxbklp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xoonqafr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ipjxpcem.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnmtqfjx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ngfdjfxf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gsbpjwkn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rukbdqje.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iwlbqsdh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sbupdwyo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ddzrqmhc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rxwjhvcd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jyyipjzi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kchgfngw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ddoybyad.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vfhqnbmk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mhmnrwuo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3duysnyzf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pnjekpmt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nhsbrcyb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3efuvetsz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iaptbtqi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gaymfgyv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ushourer.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sdirvrws.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grfklvrm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pctlkzgj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mysfewyi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3peutlgux.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sopkecrw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fsytbgdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxnnexqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3stpzbdms.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwpbcexe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jjyexosc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dolsclna.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vavxfqym.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ujzjopny.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fszejtyi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfbxjf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnmcwhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wguvaleo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fhacmsot.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3llivlsim.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3eonrygyu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvqmbhoe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uyqwshhc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zjonwxkk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3alfapnhv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jwjouwem.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zlsdeapg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3faokwjtw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zravmxqe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zbtcoukb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fuhtyuha.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xzweamqt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jhtvgieg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yknbysuv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bgizfzvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uqyosmxh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3egyhaxfz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fnuvzysx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3imgbevpr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ydmoumem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wssrtylp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yacdscrp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3sdvuqggu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ihywkjji.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hujswjwa.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3omelxekf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbnfqsqz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3roruvdti.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dbymnmos.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cnrgpkmu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mwxtegbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swcvxrdv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mrdveipw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfksqcco.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mzrkckin.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wgfpqtyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jelhweif.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jjdqzyei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3himjvuag.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3bhsgkeyv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qvorjcau.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mrxvroqa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ggewkofk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dzczsmkf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bfddkkgt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tflxmxjc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tlvvbvpy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nbbkripl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ysgotaob.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mcncrbpa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dpoegafx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xenqwfvk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qdrkdgyd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwkfudgu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tbjrofvq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ogvuqgvd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oyfxwmtu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xsilwakl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ixsnqvqf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vjxwjega.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jjaghezn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3awziodbs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bzjixjky.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3eparsygh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tapwobmj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jwieazdz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vvfkrjar.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yovrwevr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bwibeasu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3trkatxtm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yaolvtqp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dkneyzcv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bfnincfv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3carwliuc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uuljafct.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bmevrict.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tygymvjx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rveayyiu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vqaflrwh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dqkqfhny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3choecxxc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eathnvgh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mosxhepi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mlfjhhml.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzkhhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nwlpumge.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhxxbaxi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejrwenix.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3agerzemj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bpgxovgd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yrtajprt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3onkbeypx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vjimsxep.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3unnmydla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gyzlwhxk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xmyrftsz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ysxmyyqs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vlemphfo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ucptahof.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jlsvtwdr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xfnaosam.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tvpjtvyq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vadgycbz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ahbhiyoe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3poknhlpq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bogvsdgh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3hjvcnryz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bkbkjcqi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbkfvxrw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ofakfaoz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpkwiepi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rtpkozyy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3myhynuzu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ukwlipbe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qczcycff.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wvytayut.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzcsebv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ctklxdwc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sqaqgvbb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mxjeiwzp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fupfjlpd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3alaogqum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dmcckvon.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dukddclg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wavyfqtk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qpdusrnt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wapazrde.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jsgkovvj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pvxvxfwm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eiaeylwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aivqskxw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nwxnlizn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dtgjwhid.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hylxtttz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hblqgfzr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fnxhsyhm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaarotys.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nujpyxul.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ixrlbobt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ufcpdxtv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gwodywzs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qutvyfaq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xtbfpmvq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fpjkexsk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqbmtjxm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rxbsmbjs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mjuzmkry.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3holelmuq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3smitntkb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zpuicvte.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wjakiqpc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ljkzyrpe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ywcdbljj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mxhirwnb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3asmrcqcy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfpztxx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpewwen.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kerozeiq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3eqhptkcw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yyknlmeh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3eqftpmtu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zoiqrfyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nyswhgpc.html


<!-- 参考信息 -->