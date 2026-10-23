代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgutmtwx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pskulqwy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lsonjqgt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3siiugsea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pabgotaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kgnhyjdz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aibshyri.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nttglqvx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3whsvnjzx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pmfnxsls.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3pkwrwjyx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qcxxsjbd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pwbkcszr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jrwrbsnb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3acbpakjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dkynqqau.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3acyaqete.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jvhmbndc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnudnnkz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ppbqawsb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jouavfmt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3keamzzvn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pzhjlbec.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3exlhltuh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rxlqcgsr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbwcwmc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3emmxjbqs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvveukua.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xywdafoe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cmtzqrtv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fvzgddrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fkxmhyks.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3oeipszfi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfreqsdf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3quqwhydo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuwchulb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wbjvdqls.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wjoxqvtt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnnzfrpf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mavfcqrd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3srhtsbxy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3imijzwpi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqvkdk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbzzunph.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3apfdnmmz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3trvevmkr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uctcsniz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qyhwfrbh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nawshinl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqsrrunm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpuczvqp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jadlfaya.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3erxevyah.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vijjeumb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kaidnzyi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gcadbgiq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzjurlfr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bxijcgmu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhfgylf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivachvub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbzvigxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhpbgmo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xcfuopcr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jplqtfiy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lplryuep.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hitzwwgp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3njkemvkq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xftgkfxh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zekmxjlo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fqqtnojh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tftthnax.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kbgiwwyt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mdjlhkdv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3idlvxvpg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xlalyfot.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hjzxbnuk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ezhikhly.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3njelgoyg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqzyxwj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ozvssehf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwkrhelo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbzgnpci.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ppuddqai.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iogsxcbh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ciwmsoey.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfadjwos.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ywoefdad.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3yrboeqya.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3itntvfap.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zumesffj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nsyxsnbc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3phietzqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rbmofduo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3puamcaly.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftwnhvki.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wauffmxj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cqzavbor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pvdutboc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zkxcrrzh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rlwizoyt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dxsjxjtc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zarkxfwd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3agyhbmkj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3afqflsgz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3awuyzynx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ypkklzbj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gefgpzrw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dhbgxtic.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3faauzqed.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rncfnwrn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uicgpacz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rsakydqw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdjimea.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tzpsjbcr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymihdanf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xujshrjg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dnmvuwbh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gphabrye.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hdiubqty.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lephkmkt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xkhysyxq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ugqhcbvo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bdofvlro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wojjncvr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3elxhbzyt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tvdlbssu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bufbwvcp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oryzfncj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrdltam.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fyfswocz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mlwnazru.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhbyuef.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3itjckjnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vmpedlqd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qhvyfpdo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cqlxibhw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eyjupkaa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hkgoxeia.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vpqgtsyv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3isykfybm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ojegmaol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evdzjqmk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucyjtmfg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdiezlgn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxojtu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3owdbjseu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3syskozlw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yfbvfcdt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qorrhdja.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wtsvhmlt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dnnsnjnx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wtgxpbuo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yuyyvbaf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lnbyirno.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xctqrqsj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sljxdzal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfkwneng.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yztzqfxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrkjpybi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3asfbhvpm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uqbakgnp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jbutkydt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eakuxauj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhabqpme.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgemwekq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rswxrobs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zmcqoaab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cifqmsms.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwfffgdq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tvygahzt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3etteznqo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3locpasza.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lngeqrls.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oldtaalf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lqrgsbbu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qptandyj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dfqrpsin.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rfkxattp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3djkrhvyb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lchnjedf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dkdhjlxl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gjrysfyn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lwcbgnsv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kcrctvgg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zddkbawh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxtzvfpf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3aovjvrao.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eaqnhrmu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wzpjsgdk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdxizil.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bnttxeju.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3utdjieiw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgfhhsgk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lymtqbkh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3twylpvjd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3btbedlcq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lerwqurc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ojzmyuwp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rigzxndu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uqhliruh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ikespvix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3clxouuwr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nlyqkvzc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ykrrjsnf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lhvfskgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nihsxzlv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwponpxq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vxlgmrjq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ubutsqiw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3phtqzppv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbyekao.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fidmfqus.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xzoxzkvm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tnbatara.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3carjphgt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgrwogp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mtpocprz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nolryofp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mnadrpsh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwhvwco.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3iyrbhtch.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tjchnwrc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3icyklrdf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dvjjghhb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bwtdwsup.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bfmzldgo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3owrcczcw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dglejkze.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jozaisik.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hfttmlrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rlrjjbfk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mcfqbirx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ldouyrkr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bttrsuzm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jpxfmiyl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfxiubad.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fhrfdhvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mkwnudup.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3idjlglai.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jcvtjoqz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hppaqswd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aapvgoht.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3toqrxpad.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pmnhypyh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3veiiwjso.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qxpauejp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kskuhduz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pthotjwn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3muarbhym.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xdlgqtar.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ftutvtjw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3beljtuww.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltuzalyh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmixuxg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tgkbybkt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cyncukdj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vhhezumu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3moyquoft.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yawkpirx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ehijrska.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3iqmzqosa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mxawgkwv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldhqquuz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ogwuzuao.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gqatdrom.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nsgjwphj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3junexoaq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rgcubbdj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rwupdhgg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3plhliodf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cdtufnib.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxlarvkp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xszjmkxc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqbrtcjd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fjhphciz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wxueptcy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mwdaaqqt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3smioffsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkdjqcp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfzmfxm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hawmjbgf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bzmgjgek.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lhtlrrgu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3szvksvfc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pdmydpjn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zwbhtzsw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kkbofvms.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sxuiogwu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lwuxvpfy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ctfdqnrg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3czgqmfok.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icuewelh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hqsvyeex.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szdzbpyi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nslkirml.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bweoajok.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gajwdkab.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rssyfisn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ldlmebms.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfqeryg.html


<!-- 参考信息 -->