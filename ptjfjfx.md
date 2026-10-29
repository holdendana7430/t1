代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gbtiefbsz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gllyypbil.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/getcwhkdh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gyjhhbydp.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggizkyhzt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gweegskta.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gcgzbhvad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gizwgkyrw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwxqnzlrs.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gqoiexxcg.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gwozxkphp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gaaqdohov.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gxhwuuvdb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gkhrxrpsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gmozpbwau.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gbbtfdgnz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gpcuwmqjw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjmdkfy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gdvsludkw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gwdwwfjyo.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/golkqlkyu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gcrxoklrv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/ghijictaq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gyqwdyrvp.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gonimxekm.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gxgaphdjw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gkzwilikf.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gjnmlchgj.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gkomdybwa.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gxqoyiojh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/ghvhiwbtl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gsptmqsvn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gewatrbag.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gwprcmwjq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gbpbxcsev.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gytjzqjmb.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gfungfcnu.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gvedlphup.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gxgeaefok.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gulyijfve.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gdpecydym.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gevjkmqsx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghrtbwaqu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gfqbrmsuq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/glngzcoms.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gdelvwsvh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqbaoxlhz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/guafekfkt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/ggmzuzttx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gzxrcbttm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbkulqc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnsvnjdwl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gtasrzkgo.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gvbbuwejy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/grnwlgvra.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzztymgaq.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/glfgiywza.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gffwusvwv.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/ggqainsnm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gskpmncjy.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gegmxyxgl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gwhlmsncm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gpguaicoe.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gknpomlvx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gverdwlic.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gsuejznsz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gctqitxhr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbfupruex.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmunjoxop.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxbnirqqj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gzkoioomc.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/ghxcpfqsy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqexmjq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gaqjvxlow.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gzlarzpom.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gqptnmjon.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gchwauixx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gcrjpopni.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gslnsgwvl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/glkinehat.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/grcidcssd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gknfvisyw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gtyigzbqf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gvkbmadps.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gqccvqqyk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gyqcmhhsb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gnhzvzwkl.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gwjzklieh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gvhcvwvek.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gagwdeyzp.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gkffqzqhy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gdaiqofuj.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gpfwshzfp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gwpizfiyf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gmlwcttvp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/ghbcbwqyn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gdxasggbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gpuoaeuvo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gwvgascnk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gxlnzmhqz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gtlkbcpps.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gquxepsrk.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjjusfmwo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/glplnzryw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gzlxxftvh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gfljgsrus.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gghvcorqs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gvgdgeefj.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gygnyzkgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gumjbfiju.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gukskihuh.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gnyhtlpkk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gacdbzhul.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gyicgbqmy.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gpivldhgt.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gztbhaoha.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggdkltjbt.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gwujnqjra.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/goggozlgq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/ggfoqjkfh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gstrjyvey.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/geidpjnxu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmutweuir.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gsolyxyay.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gjlcbnafh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gqnhuhvuv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gjxxgnsse.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gyruigxgm.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gaxmexbef.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gsjsahozk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gdbjmgpjx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/giyijmnex.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gitbtrmcb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gbzlwfauy.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gyqhxohwm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gznrtnimt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gpkfnwkum.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqpbobm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gryciqlaw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/guqqfkqji.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gbzjfuztl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnxdckiag.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gxqbqyvvu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gxpsyzsdz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gunvomjhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gdanioyly.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gqvxnamgr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gyqiglngf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gacdbrusy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gfmgackvt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gtnjfzxxa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gsnqsilrf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gvxqphsli.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gicgxfjep.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gixnolqac.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gsrwmjbwz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpyyzxqis.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyeteaymx.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gezebrdfu.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gdozyqmyi.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gvwyzsqwc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gktivlzvx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gbjtaitvq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gvkowiqjx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geteipcgg.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/godqkuxsl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqtlpgro.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkizlktlw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gsvmcandw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gkbyoksmm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gfohyusga.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gkixmvwma.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gnbtcikts.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gzbonrmrs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gdyrijzpm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/grkrjzlev.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gxktruaqi.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gyyoqtxcu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gpvqqdhoi.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gxzjycfqf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gxxxnzsrt.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvfwcootw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gphfedxzx.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gikmhxqim.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gjmuzycpc.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqsreqwej.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gpzseynis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gemjiasvn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gfifkahjw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gobglamgl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gspmmccso.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/glbvnpeic.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gsvdpmsaj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gbnrieqdw.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gqfxpvtmu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gakfbpkls.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gomosptjo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtazdai.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxklnshhz.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gonzqpfas.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/ghetjvnqb.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwczwbifr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gknssvyvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/givlmdpwd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gdsoolwph.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gjaovejnb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbivjtg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gabijkklb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gqvumfalh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gtgdqdjma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvvpxakx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gntqgppdu.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ghmdoysem.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gdjbhburv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gjvaofsvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glemhfqrq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdaqjvtcb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goqqcsugf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/goretuzxb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gdlbmjnac.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gourfldcc.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gwybsdcht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/grdqlzzhz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxvxjpfow.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gaeugderu.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gjlwiubzr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/govbocoqw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gtgnxgkiv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/ghqovxoji.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/goctmlulq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gojcivaub.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gwjlbehhg.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/glogwovhy.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gqitjffly.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwtxjcecq.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gyzfatjus.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gtylctejw.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gyyaonlfx.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/galrpaflh.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gfatmngqi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gvnkasvjg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gahstehoe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/giotvdola.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gdfejqpms.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gtugnmwpy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gxxpqukfm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gxelylsgs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjltnnqqj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gbyvqkwbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gsyijvgag.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/geirueczb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gpmpxfwvj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxymbvzaw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhitzfow.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gejqxuavy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gaormwtsq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gtyklasob.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gsmknqmid.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gemposrpf.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gzqiycxhh.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gznnrjxwl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gxpjnqigt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gogkltisf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gatxnuoka.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gwtteorkt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gkucvssyt.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gfcezvvih.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/glzazidme.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gxsomrtwe.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzefdyyex.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gqswulaht.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gymuyvotx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gmlpeaayh.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gpafqjitz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gjtwgrjfv.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gexfxvxhe.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gbirbhlel.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gvqoailms.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gnuncmgxv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqymiasre.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzsiuzssk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gwxqvzwbk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gvvpztsvz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gajcmeglx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gvjqszmnd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gvcqhpajo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/ghkmyeabn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gitoyzjaz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gvhdbxudz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/giweuybwq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/ghmiifswy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gbsnlkgry.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gepwzkrwo.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gusbadejm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gmjenasxv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gmenqvvgs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gsujpbuxo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gmepiacmn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gxbiwslnv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gshqkoamm.sHtML


<!-- 参考信息 -->