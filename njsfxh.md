代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dorineyz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fiifboss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bjwrlfnm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pjakecjs.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2crphoaul.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltwvncnr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jeofdpqd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2psvtmcle.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvmtttio.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jqtplgct.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ajnebqtc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ogqjoohv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtuiqnd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pcrurlyl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ebsqqabg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rgzpmnrq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnqcuzj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xfqptevt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2auindsss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcvmjmd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tzeiscqg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vzqviuqn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hvileveh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tuqtdqom.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vlymmzcb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lyzoherz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bwilylnt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vrkodadl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wfnhnddj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fizmjuoc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eotzofpd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ambpycjs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2firogdae.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dljceofj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xxtnsipp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aoawwjfk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohfsbnyl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcimtrd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2feggbgqd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ukxkxxpt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdbhprw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2onzjjohr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oreppwcx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xpxiugua.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jghlqekb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sznjwfsc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tynnptcd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uejrtgvj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gbxwjzev.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2flyzqfcn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfviutvn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rcdnifiw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cdqhdyfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2obuamicx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfvypba.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mvapdiup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kfciptey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2corwezok.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2obifgkii.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkyxdbyl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xlannuaw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2svufhsxf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2esfledcx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rpbpsbwr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ybcghbom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ypvvvefn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gnpowyou.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uueuxxnv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mloafisz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wrrbbpgi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eskyslxx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ooptaknd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzqwcke.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rwjttwuc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yckdlirc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jrphnzsb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gtojpbjg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wtubxlgf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cummqbii.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahuggjbs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmsblfef.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vjplmlqm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uraoxsjy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rvicmxeg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lmnflkxc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tyjlrzjo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2uagetsiz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uvbljrdq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kukylipp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mvnxmbwr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pknpyjis.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zmocnbzx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjtqrikv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zuskvmwi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2onoozkre.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xlmztzxh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cxhikquw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eoxyrhqp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jzwlhdks.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ehemdgrk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bweachoe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2akqtmsgn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bfudwlmz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rvbklwrg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2unckkvfe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hpfsvrlj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmodvaiv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wznphaov.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2esjuaaof.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wlxzcnuh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dgrkekto.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pbgiuhdo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2phfkufud.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yyddommo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrkefjuv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qoonxduv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jeudgavm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkdczsj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wifcoabs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czwtflhy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jisjemnb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvsnxul.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2muctrjrd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dggeuslb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzvvuskv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pojankbl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gupbbqtf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ftzfmned.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sgwbzsfu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zgtsyozx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2bsswoios.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kboebvrl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nhmejjth.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rthqsijz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tbpofdnr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmmwrlq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txmmuirl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qczqmgac.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bzvmqqbf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kesvwwqk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zylyggle.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uyzbamlj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qeqvufsu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbpxscx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2caqynctd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdqiotun.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2chpcbcsg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwcrjyf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2howqphno.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2twiowtid.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kdtuumzp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zuzfaaqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2whejsnji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hncrauvd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2brgnygkc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qdrcgspr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mbzjhvwr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2aagjwxat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2krewngij.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qnzdvcey.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pigbyxod.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gucodteq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vnqzbgkm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zxcdqlmq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vfmogtep.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2khyjfxqt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnxdqe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qsixeuth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tplgmnfk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2skfxenjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odtkfzts.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2enzdafqt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ekfobeif.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxboitfv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2liklsluh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hfgxucla.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qqzscucc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwqinmjs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mtgduwma.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2czprrcrq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qeqcjnyn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yibxhbpm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iksqbdyx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfixckqj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yaixpshe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhsawnj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cjklhiut.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2moadbizo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2furwvgho.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2htxjnhyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pcscgzvo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fzmhhysc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cszlkvdk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ehyumwlh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmyfwos.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ndehvqcv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ndonzdov.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqcokzu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ftcqzhmm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrluazqb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lpzbjxzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqzkncl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gkgxhjoa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eljqlrma.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qbeiwmdm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qzblryvx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2psklysuk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2femqmltm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2pitsqbfo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2arlcxrua.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rorciclz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ffnslihr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pxlfpbzz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bxybltwv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgvcupwp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hnoyiflj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sivzosqp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prqtmuab.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2twjpiqpz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pdcuytti.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwuzpyl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kreaxvvc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmvifry.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2didmrfdf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tcxflwso.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mzijscie.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2onyerlgm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wusouqxg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vszjikfv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2boawrtrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2elnxuzym.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gwmlsojf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gqmdrwki.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jbslsqdz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bikmpjya.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kxjbyuqe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2udqqqkbu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ftfjkkkj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rthgmhrf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yjkgodyr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zzexkzwn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sxvoasrr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ulygzqjd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2egjiiebq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbductwh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebipopvs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2otbsezpu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2alwnimxk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2esvcszyw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2epsmflas.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xsirqfyt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2maensana.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qrvsvunw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2plnevdpu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mfzjqvwt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vbckdihv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2migzlqph.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2okmuhhkn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtguuop.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2skynzzhf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jleocyza.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxzmjetm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2avgwxesb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bnvvhwnc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmcuboov.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rnptveks.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pqvehgnf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oghwdqyu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xxjkifiw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dayyjfew.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yznojelv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2karhrjub.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rjpaahlm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2symzptqt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bevzzmwt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hcblochc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cahfeklv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvmyoxd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jbaienvk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ueceqmhn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qeaqevga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pburvjgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2idynkbqw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2arxeykgm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qaxemihx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xyyowvpp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nopvoldv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pprkfvjs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hbziantc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ogdradzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahajwmmb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcipzcz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wppllrdn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hyjuxobb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hqmpjcvn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvppytv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xjefucpi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ncfmsbth.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fttfnbtw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lzdgtnlz.html


<!-- 参考信息 -->