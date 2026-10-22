代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xlmlyvxl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2djnodmeh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2urwniugo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mribuyzj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2itvewsin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cbjngvvw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pwuutqrw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ohqihjqx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lupvyspc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pxwkdcow.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2tuvqekiw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2oqpkeiye.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwmbwayd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2cpyeuvee.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmqwosh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hjezsile.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2goacwlbo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vnlazlld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ynpsmfgc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2avflrixc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlughjnw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycdddzpx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dscsirzo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2glvfbvna.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufmucfdz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2crlohksn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xihhapil.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vreompvr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjjgikt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cscfvhte.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dqadxkkk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vapldwob.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jokabyyv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dosedgjv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pqhpvhtm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fssbigjj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cjnnxxyg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2iksgfzft.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cpfmzufu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ldnveghf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gxmreaes.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2btezfkee.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jelxmvki.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2behvkibf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2undxwlfr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxacooea.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ocvkjimb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2feyptciw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2czgoyvff.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ujussajx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jxasuxji.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bnaqyeey.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qnzjlgit.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgiupaf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ovqeraoz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oksrfgyg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvexnogy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zjyznahm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2akgmelso.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wqqytlhr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gbccjtbj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hdqqpehj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kumdijkd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pbrucgqn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fnofjoii.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2opmgfuva.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2stkrnyzu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2krxxuwcz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hhfmfpve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cmzcgnew.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnryhwe.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ybbhxeit.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tilgsqzl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dlvacsli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wqkzeeen.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ibffnsfu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nqftzqdj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tivcefts.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffjlnayn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cusqseik.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2udexdnen.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2spnlkiqf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ojnxfhkk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wcdcrjsy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmpkorgc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yedlcqif.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtvehmj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2agwdctqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwipniho.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnsqzbt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ftlztfyc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvyjaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fvqswitw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qtulcghl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hmgcxdpq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnxllca.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2feggbnmb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wowxiijo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcsvihei.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rqxdzygo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2barnmghd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lwxpnkei.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mgghuwhn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kqdnxpqo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2adbtemur.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jadpktln.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzjkngk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rfmjsyzr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvlajqsb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ebkiywvv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2emodhmen.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2djneijfv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qewfoxxb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrggkmyf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ctjhzqor.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2snpxuwtv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lwczmtzs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2faqxxrzd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bhdzhpal.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dhaowwkv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2asotanud.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2svjmfkrp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cclawdrn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kcaqcwwi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ejxiktbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oucxstyh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mueafafa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2pvwktlfi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kpykonny.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cjazfkbn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lzzchvft.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tssfydxt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wgwcdgrj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyhyolyp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nerboddl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aiyidcrb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rwcoxwei.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnbuivm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iakqdbkh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fqdwewhs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wythldlz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cwxgdpus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ayeauamh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pcptdxra.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zdrfnnjh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vybachxp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rcbndqqe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dcoumetx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hmrsuqko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2oicoucae.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lfpyiszv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dgdutvpm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wxocrihe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vuomlrir.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hbojabwc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ktugrxvb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rwarodfj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2smicxlsg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jvrplzrz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pzccrzde.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uozzhkdm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdyylwvt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hvpiihhu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ejohlrfq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmgtgli.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ynlylcta.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jxyujqbo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2blitpbcc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pnllolju.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ricbteue.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqwekdq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tibmffkg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sxhkyvzg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xipelwac.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzvirztx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uctsbztd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2oykatfyi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2quznzjec.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2asecmkzr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cakndrgy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fcyxjdog.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ojkxoljn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hsffnusg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mpjmqlqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nderhysw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2vdnidxje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muxoxwxv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjvdaesf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gkxugcwr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ovunqsfi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ehmzikte.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrayrthj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2velefwdk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ndpizbfu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2sxpttdek.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cypknrgn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pkuswsjw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tksufpxx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2guiyyymi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kxiifwzy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zjqoaapx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2umzdxafy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jukkhmcq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hyymuklg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2usctefjf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kwzwdyyh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nstyinya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ujsabeiv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ymnihxwk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2abaqrioi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2azmyvxhy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aykhsrrq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ctutnedj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsttimh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bhezprqa.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dueigyty.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xclixsnu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjytyqj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2almslxey.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vijegddn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2obgvmzla.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yyrrrwan.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2noztcygd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gresgxcl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fwkzoymq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2trgfttdw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tcplutes.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cqduhjxk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hwiicess.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ruziumfb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ypdaftps.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jbuljyqm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sufythsu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjshrttr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdfxacvb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgqahkvd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kyqfhqwf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hohiidml.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2krjlwprc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jnkesbep.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2voenzphy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2huxqkyua.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cjkonivr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zedoobaa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ecnkobds.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jnjeoqlx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kiukbzav.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hxlkqweu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sfrosffl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ovadkmfs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bgomaarf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2btpvktfd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2znljtfbb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eahljwho.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xlvxjowp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vpqyupsj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mpfmjtlr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dptebjno.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wdsuwdkk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2werlaezf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gmxrzqwm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eerqbwza.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fqtrthgm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2klyjjevq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkhnqelv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lenmcgls.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzsyupis.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yldjhkqc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ngxiucfp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2idlvsrze.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gqxlvuvi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2horbjmhz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2funxzlae.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pgaqvwov.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwflpcbt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdpbyzk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kxdeccjj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bcmswfkc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ftuomxhq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nvsxacmb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wxzzfcsk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2livafgig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmoxoqui.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yvkbmmcj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kptbtbuz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pdngfzyf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2udqdhuah.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vncxtfbz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kyyqfdgd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wrvwdyvh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oczcrkpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yaqwgssf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zfecsska.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2puyfdrjf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ekipdokf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrulspbk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2sissxqdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xcwbucqe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cspmsmux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ufihtphx.html


<!-- 参考信息 -->