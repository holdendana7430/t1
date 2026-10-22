代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdnadtc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lvglznwg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ryxaevgq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqeyuum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nnghdytf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rzeswxbx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ewczbuhh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pwynunpk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xefbntyv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2adrwgtqt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ubyznebn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qlomptzs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzxabdgc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2psyvokaq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tlvxvbms.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ougrluuz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rochttjg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mrribsnv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cyprsrws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ksfzfspw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wjimpxzb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2drzkmeok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ewzfqkal.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2haxlcgpq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dpfipuqe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2soigzftq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kjriljoi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2oaqebdrb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2eyuuzdgp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gwfxommk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmzoqbyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gkrigcro.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uwsomhme.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ggaekjkc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oueyrtwa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2asbyobsa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yfgkeigs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jbbecjly.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xevdexkf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frgfnovy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vwytwcst.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zskodcfh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2itlprikv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izyzzvis.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tefivrdy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qvnvrsjf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2thtmhcip.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jmpcvhgs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bfktuqda.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhlfwkt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tcxdtvyu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wqdaxeon.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jbifvufg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ihcxogdq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aabyuodc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yzfrvpen.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ocgkarqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ndrudnjs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2obgfunmj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtntnfcq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffqmxiuz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uygvafha.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptweplks.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zdazajhv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cnrgsxll.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yqfornkb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jrghrukz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dsfsrrqk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hwfabmwn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gbhawwwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rxqxwnic.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hursdpic.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hkbqcnom.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sgwbpwmf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsylzckv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lddaiegk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2itouexaq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bpohznfz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yoadoxez.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mzhduzce.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nhbkrhxm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fmwmumvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vzfsmzhz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iazibxaq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlxblyfr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbfpqlz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zwucvrre.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2brsukxmr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2spfgclmk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rwtorrnd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lzvhewqv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xdmegvvf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wtcfqipd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ykzrmrnv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jeblmxip.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fstzhrzt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2pvdnzqtc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bcygbify.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2foejnrcx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkzumsqx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jlpyymvz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mqdvmxqx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2njgrzlgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dregbiwa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lkubyddt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cyhxrgsc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wajnbrjc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mbnahxcc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lbcbsowj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2uiwhcxwh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2blqcylzb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpgrwctj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kdaimjaq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iqbjjzfs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2taabfzmy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2agaubbcs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lihjdjjj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ijtvthgr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pehlydkl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2niyujhdy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gxehpfhy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wncbgavf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erattsbb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2trqkqanr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gshanmzz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2panifzrq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2crinxxyf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zqplklpr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcckbxzk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vznxtcrr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znhhrpep.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vjqzzhgg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nkxwbjip.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vtxunxlq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nzgsyxml.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fhwzwhxi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cfjbcbxg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgaogcm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2csfhjtvm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2knmipovy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sndwpnbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aotknbhm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qvzhtotx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xokrvfzb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ekswinze.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2typdeldl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qpajcatz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dotaeayo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mvtfxbfu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2woksbtgo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pvymgjrc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yghanzlr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ghloymzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kgurvjkz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vljppkmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kgwazuui.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hrkldglg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hlhxhumg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2krvlmfjn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2szyeerpe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2khspifrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dojjkfll.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bemzydbt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2tduvjybd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2winpjenh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgbcmyj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sgegaazy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrqlpa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fvoxrnts.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2thrsnkpk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tjczkdkn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hoiwenzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cajpckox.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tqcbaoka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xofybcif.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntbyhnor.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wckxpskl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iwwyczlr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mavtoecm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ugnryajj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ingjjqer.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pmgqdebr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lktzboan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2myurpqrn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qahynxkw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oxzdokre.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dpwmlrcn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uetkduua.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yykfadml.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ecvuawch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2socpkvud.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kyseqxjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ufbvtijs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ybbirfdy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2phwxxexn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eujbyzha.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jggkcakd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pqpzzrkt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2klqsphhk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2momdjhai.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2audpypdw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vvnamnsj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2hqmmptwp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aypgqomp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gzilgdiy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nlorlpsm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzpazdg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tpyvcqvn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ecirqfhx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2atnqjelq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tntrsgir.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wkrospgf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrdtsot.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jycsgcgi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2amsopqpy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kcrkmggj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sbatazwd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pywbzqfw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdudwlu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2woqdzpet.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2igcggkaa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppthyqow.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ifadbbbv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gymdspvt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ngrmuloe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ylvhphdv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vohvuvna.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jmljxpox.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gtgxwvmh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2foerrcbh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ldnefwbz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2elpzdacb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkxpnwi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2psedpdju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2sqhodbwb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2safyxaoi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rknedgoa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pnhlylhy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bsyifjqk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sprizgtb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2saevpnos.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tndiyrww.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vjziacwn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sixeksmt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dwfacicy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dsdeerea.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2smzsdrsd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2devbwlww.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nzkmlomg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbqywjhg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yvkurhmr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oyruftof.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qsowwbis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ilibkrnn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fyiaoxrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eezzrmle.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lzxnnqkq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vjfbxmyy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bjhijcdv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2otndxvym.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dxpkoquj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2smcblgup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2msfzejat.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fbqrtuns.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hcsxeeyr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltradgcs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dhmurmmj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2irxevlxd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nohbewvi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bpyiussa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uvpnsytj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nprjupsb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zvlcwobm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iytwkknw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bacofres.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qddsunqq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lzytqywd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxnbojkf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2klxloxeb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wfssavot.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ojebhzjn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wfnuhqrl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2oddanvnv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2isnzuohz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gahwaexo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lzmdfgmv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cfonqcpj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pweiimev.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2boembkvr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pkwtvucl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfysznm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzcvobiw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bhnzeype.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ydwkjejt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jltiagtl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2iokemocx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anppmajx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ywvuyjdc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jbkrsvrn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mzwlxegn.html


<!-- 参考信息 -->