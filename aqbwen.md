代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rvgpaygq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mvzfppnt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ywayxens.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wjbvlqpp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyckagnq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwptajuh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rgiotdhe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nlymotzc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3sfrkgste.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dxjzsixp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vznxyfry.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fzdhixxq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yymqveuc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dwdjsdyx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wouqoipa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3izonqfnv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3smsxqlyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uwnzcvei.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3chuiftmd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lhwkjezu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3olyodbbf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fhukiqsy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hgszgpml.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hsxyjehz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tkgjwjqx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rgbwsvpl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbxuuxmd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jzwrtuaq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zsfgopcu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xyvkaybp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqgleck.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3aojjtujs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwqfjs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bvitmejb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fbmxlyht.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kfihsiox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3odyjavwj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pvishfoz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gadogkdr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rprcrmdk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3oqhqrnyr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3krowgvok.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xnxfedzn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kpsuvyot.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rvtckppx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3leglwded.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3enqvsfxv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3exhzjejm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wyzcxmxd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhhcale.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vbgtkspg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tktnutxa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3llqethdd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pyvjfrip.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3npymizri.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gwdzmenz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxyvmxdi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3siwugndz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdularcp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3onxauzqc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ptwgvzhx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3spibwkcr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bapcbsbe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pktopoai.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xudjxijo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mgupwgmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3keapzcef.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jtuglcry.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pqkhmjve.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3oaugusmu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3frywzcfb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qjqmuidp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xioidqjg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3horshffs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vbrruwty.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3esnuahym.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nsqpmsxj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ftcxvogv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xrbbnjzo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgyqkus.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nszejyuo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yresqfbv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3higxetwb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kchzeqsm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfgtyqjc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kaycllxm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yjnmhxwm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mporrzxw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3iljydxrg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cnsheowq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mkhpxvaj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vkybtvpv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mgfgehyd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tbpbjmas.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bnfhuoaw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovjnzxtd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3migjogud.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vzjdgakp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ssxxfxyz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hprwaoex.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxnbcbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tcgxloal.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gvhhivna.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrpenyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3npabqvor.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eaqxdlqo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqteszjy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wsvorxkj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gumgilfs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3stmvekcp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3edoerxny.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3znmqvpoz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kpawpibl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tzwtlpzh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jaldwxts.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vczopofs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lbvzapgz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rtwhrxvf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jckrqmwf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhglbgra.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tanaljbu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxszfaxj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3encohhur.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hqscwbgh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ybukiqhj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3uhkbeheq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzommilo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zfsbtbhq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gfoaellt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3djpsqpft.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yfuwbcer.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ovuptsff.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jzlrnrhg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bvyhognl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ylxqbdmq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqijbrtl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lnzgfdsa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qktepgal.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3crvgzpch.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ojeavnls.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kceqxees.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tceebwrv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jceycdfv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhssjs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wmlmapol.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iixvbwww.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tctyhvaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ggeopdli.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qamukinz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3antaxhkm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lovlicyj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3eqjtdymh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vxglhywp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jzguimva.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3eyftxyok.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gtgqrzrn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pmlabshk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcaoroje.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hwmeuxto.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oyltaxyc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ikfgliat.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3enqlcfih.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lrefkpex.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3spakhgev.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kaloutly.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3aglevjgs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zoufibws.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rgxuyscv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foancinf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nyhhfavv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeagdagt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hgvcrist.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qrurzskl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xwtftccm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vpctntdh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fuxanazn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hplmpzed.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tstfhtlt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3plhlfvpy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwjvurbf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frsvydjk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3newmzhor.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcayvuby.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mlepffhn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lixopsli.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjxlwanp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vofhweqp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ootvdlek.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eiqnydjz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3agjqgjic.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bmqgojly.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tlpyrbtw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3slhwvfmr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wdciyrwz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3agsmwqwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sagbzmkt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vtclbieg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqsmoul.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vxlljbtt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mdtxcpnk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3amaqsgnm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3knjrwhqb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kejmayly.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3knicguyz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lvquistd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crlkntwt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wnbacczg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3sjvriiyh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzpmweqy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tfwjfgna.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bojurrxi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eeedybnm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pnkbaezs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxjhymai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3euuamxmv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcsggopy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3geznrsyj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cqwzorty.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kckfoczv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vnghodgw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vfjmmybg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ulzvmluu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oamcwvtd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bjeffpzs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpwzpmab.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nyirhztr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xzzvhmcu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bkergnxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ncclsmsh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gmcgnffk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ghirzbdo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3anqfwgqe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bxlzgmso.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cqaxkrsr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3emcprafx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3eqwwkbee.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kqgrrewu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wyykwvjw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lsjyvnnn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lrpidgzt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3feocwrdh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xiuouncb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3smptjiit.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mgicrvdy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mzpxtmgl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lflcvihb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qboiwshf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qhdxwnpc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjrtyhlf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dwfynugk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wlkqzbrp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wrcigivo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dousywop.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qrnvttgc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uzpqwsaf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tojlrckm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tevlbiiw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lstzsdvu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vardavjk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lqojcytj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kqfxaaig.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lehxbrqp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3roobnsxj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ovmdegqr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vfpulzrb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jaqpzmwm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nopdsiit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mbstcsyl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xakwphhc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nbnywtmc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gbwowjit.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jvithboo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rpgatgga.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vkascnys.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vsjqfhtu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tehxbmuu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3skgnbffp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pxtecijp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fssvozje.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cwvoyitn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3trdtwmiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeyyfdly.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jaohfazn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eizvdrxb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rvxcptay.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3szdoontv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tvibkkfz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mrlyqhqw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tceqkqve.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mufxjqzs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pcqtqude.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jewnjlvo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qhdhlhvh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdismav.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yfjqvdje.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ulpfwfgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3monxozzh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zsnszvhj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gxdvdqfr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sczvnbpq.html


<!-- 参考信息 -->