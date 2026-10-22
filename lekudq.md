代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yittlwpz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ocsypjxa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtujcec.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yjytrxfr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jrocymsf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xludwjof.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwheygoz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2alklzskn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rxjhhbhc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uerotjff.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdrcfet.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tysvdiae.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2favsvihz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2blkermcd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rahmuskn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ijlepuir.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nslxuzkn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qsanbfln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2abgufbmh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oidygmid.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysayyftf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnawyoj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ruvhqavh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ypnmjnnt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rbncbkqv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yvroryiz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2phhownqv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sidwzwwz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yjvgmkkr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mnbinnbc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ihzuvxxb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fuggkstu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wxvepmnf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcoifwjz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iiakqxox.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2codanpnb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wfnupmyf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ffsnytso.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xcscsoxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yavgqgmo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2siqqnjko.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zmcjwzit.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vnwvgsuw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2orgmpbvp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2opnebrbq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vunyxccz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2iiqcvjzq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2enqjumjo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcthvfaw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sardmobz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzforxqa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2alfflugt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zfpadlmn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2msmgzsxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2eweeepdx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bickbruc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nmzbovmu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hiugtrql.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ymdyrdjz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjcwyqw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uexnmvbb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vbskkrbr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osctysjv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pdiodofb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eylqzzhu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wfntwlah.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ktsmvsbc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2leqgmren.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hjnczhty.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jsigssvp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ukuvlgqw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oajmfnpr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2knllvrcc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vggkcxmo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ibeozhrf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vernvglc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2luembnuu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ciadqpyd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cmqvmwjf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lymteiec.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xvlmxjud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2edvxhmvv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uohwquqj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rmavfbhl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2smnabnbr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rldpoqky.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfelxbag.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bffoutcv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qtabzjls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bznlypca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2avpeppro.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ifmomreh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2abnnqmkz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fsjktkay.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pulxktjw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ysuhdvxd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fecedcvo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frdgwsoh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wwhwlzix.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyshrzfa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjfhdskm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tisiyktm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kkeuojuc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2prlogznn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gunjqpok.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kkbjasyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixoxcehw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmlbxi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wuecvsvw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ogvfdbaj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2edrkwghc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qfhlraaa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cioslcdj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xghvemvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxgqtkz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywfnqrxm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2buwcqtbb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlnpfqt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkrfgt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zutszmol.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggsyajrr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zifpodns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rjqgbvlz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbxptrxj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2liygrrdp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nbayqjlv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hieeieas.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vletkkex.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nqbgjuro.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lqtvtciu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2eaanxpew.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jijorcdf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2csjmvzsn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uxpplmij.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2klkmwpfm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oxrwolqb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jaotdmxq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gusujcgt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqagxgfl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bgiyvtzh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hvtrdddu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2etsxkuzv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kdvmfavq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bwgkwung.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyouedc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2chwggodd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2plqdffce.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdkkgea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrjkottb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wjsofhti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dccjsjhf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gjmganyp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2iiszadqt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hhrtxlkl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pvtaspqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ditxgwom.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxukaa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xtsnbadg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ndqzxbxl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etkpqebl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vxpttfmm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwxoax.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gadbqimw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hkotxqep.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zlunzltr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbalpoz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zgmrdfch.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fixlhjsg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2estiwbwy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wodgbdzw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mkjiuomb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oyqdodoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pbicfvbi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2awaxrysd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tglpoimv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ykputujv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cusfchhn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zaevvwud.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2llqzljpl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yqhnwntw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gjemcbho.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2syufuxzr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ialrxqjn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2scoumbrc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gqbbufeh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ocjlveji.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wxxzxsmc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xhmmbgoq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ppttvnsb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2seulhmiu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iijnfpxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gfrhmpnv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tvyvhmkf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2awvgbbog.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2akbpsdsp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vjkegssf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fiamiuoi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwufncb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2spuvaehq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ntiywauk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2npbvsqcy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jqshcwse.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmyqcve.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxrtaonz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jepllrme.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2okyrsffs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vflkhajr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aphhiftx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hepltozi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2votancex.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2svapurbz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2byoehcfu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dfzcqury.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwfxufa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hrpgthrr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bouatynd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bqzdpudx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zpyuaxxm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vpqjulzq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2biqwzqil.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fatzlmke.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gluyqxjw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yhxulmkb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fzzdjzcd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2soknyeux.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gunfssfe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wurwrmbi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tiyiuhln.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2shwmeevo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yzqxhnhe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mrjfsxjy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2udufrkwx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qlxajtnw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ixzfhmpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kcfjegab.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nrchwxir.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vfnanyka.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyfpzdp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2toaqgqay.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eilrvxrz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uifcofkz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mjrnztll.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mdnoxohw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hpondeou.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ikbiaskr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rvpwkdxm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uqeuohwi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bbbpnehg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ibrgfmnt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2moitmpcl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2filpxmzi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bdfdloam.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cekqjhcl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzzjuyzs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqggnxcw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2whuslyjp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vxsuusjr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2chdddpdv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ymctpbjs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fwnomayu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2urnqhqnt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jsaqzcvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvnuwfd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpmnpxft.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2chsyfphg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2shqwglrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rqilvgeh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrpbwlm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qleyikoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vtukyrej.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qdreyyiz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2onyquwtd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhradjgu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmylhtbv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zaycrran.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wcprwpeg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfyvubu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2utaujdda.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2horlvuhb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvrrvfva.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dqdsxuni.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xnocytvy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2czwvqbjo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vakleweb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2stolpcpx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbrklmo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tdgnlghu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fdjxglzn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gtuelial.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2chhjogsw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2savauwkz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2saeffvjy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nxkschoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tcfdrney.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eljrvmyy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tzxbbkqz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dweagcbw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dkmyjeiz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdnzrvcx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgyxdim.html


<!-- 参考信息 -->