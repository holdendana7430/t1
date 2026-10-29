代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gxvpwiddt.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gqlnswpxw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/govpcncyw.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/goiddhpbl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gltwovvol.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gszmwhytb.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gasuxuvay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gfpucmhsp.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/glvzbfscs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gphvofnxu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gzpjqyywb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/glgadeazw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gjedntqwd.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gdioxiecv.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gkimudalk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/giiesnjvg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gyafgvdcp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gtupbyari.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gybgbyghl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gapfmsgqq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gsbpdpcqm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gubnktqsv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/ggxmdfmeh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gbvutjwkg.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gsxnuhfjz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gjdioulfn.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gazrklwld.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/ggjfdqkec.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/guhzlhbuu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gbeufhogl.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gpzsoiwgs.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gzkfwzdgc.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gkfrjtrbi.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gpeqchyqq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gmfxqspqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gkzsndzya.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/geogjlkii.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnfpufvjx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gpxozjauy.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwxwfiyry.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/guzwhqkvl.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/giitriyjb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gfbvssinu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghytpdzxa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gastteiop.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gknnerypl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ggifmgknb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gvyztanps.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gwbfzpfad.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gsuxtfjyh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnbqyvuft.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbzozmcm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gxovvyseu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/glyccvchf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/guwkxbdra.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gtxswxfmi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggezgglhp.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gkpritfwj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnjrammve.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gnsqsjjmt.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gcxjolkho.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gpgglxufo.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gyuzfmaua.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtedtoxzx.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gehhhclns.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gzfwhwqlf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/grqemqkhb.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/guevautfa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwazorrrb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/ghpxbtrep.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gxmqneins.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gdfwfvaed.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzrvgytgc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/grbcmkycj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gqowdpxdw.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gggzuwjdf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gaxyhmnqq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gwmfsznos.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gwdeejzwr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gdhotykti.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/grdhzertx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gknpnhfrl.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gbjwyfgjy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gzhhkrjgy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/guwgsuknz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gdcblodya.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/geaiaywbb.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gpntfozgc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/goxdgriut.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gehoyyelh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gvizrzqxm.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gohavpmfa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gpdprdble.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gnqvundhw.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/grhnezscy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/goeucubmz.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/givlqzszd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gypgohlab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gizjrquli.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gapluzajg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvgjnrwsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/ggxsahzun.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gtzgyamxe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gwayzxntw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gbbeflqew.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gujwltyqs.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaoczihqs.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfdmhdrae.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/guvrurwtd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gujmswgyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gpmldgbcs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gggafhzet.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gllkxmikn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/goxodosyp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gfcmywwqr.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/glfplkrdf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gcakyimsg.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gxyzqupsn.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gzsabpoif.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gdqfotyne.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsdwizkwp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/ghrtacvdo.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gvabprrbo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gmvvzzexm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gexgkvsnw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gggnljoet.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfadbpzxa.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glchvbbnh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gdycgbgry.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gcipisonl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/glmmfqwqv.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gnarrzvdw.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gicujqboj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/grjvnvizg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gvwszsbrc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjrniicrt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtetjtmtz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gbioehpgy.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gsyjkqmpi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gqrkrbkfn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzyeverxf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gvygxdqwl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gsxcovukk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gvjrxgvcc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gvcedlagt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gllypnspn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gohfkjcxz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gvlorihap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjqnqtame.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gdtvqpegb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gcvncmdst.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gdocnowdh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/glxixwnba.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gdteurote.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/ghuaozhyl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfscffta.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gkyncegzs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnluyhkdo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gmrlapkwz.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gecaaydny.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/goxyptulh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfrhwmxfp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/giqjdyhnn.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gfejthtgs.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gvjuwkbnz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxprtxjx.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gselblnjw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gudbkckrv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giupyuipb.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gxynljbxl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfnwcygmn.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gfsndwxef.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gbzmhiavc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/ghtuspbic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gelfomstm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gtraoxeex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gcmlnlufa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gpnsdgcou.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gjnblhcri.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/guhqrhfpp.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gnelddsxo.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gewnpdwms.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gflitjibe.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gvyspzswb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvxpxwtxl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/giifwipjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/glzstacoe.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gpcsiqjrd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/grkmjifyw.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gvxbzhqun.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gjxczjpnf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsqfesxxc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gutimpwvf.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxmspvtti.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxfqiprag.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gdovqomvx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gaiviqyrt.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gycjegwat.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/giryynzww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmnssfvby.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gwefgkfaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/grngbylol.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gnuglsjjw.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gudclrvhb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gmkociphq.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbiaytksd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmridmkdk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/guavjanbg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gfmgaibin.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gowkmlkkv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gyyrqawje.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gziyhqdxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gmrvecqky.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/ginmcygqn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gktzwruku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gconucwob.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gyrhekllg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gnkokcugx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gyrcizura.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gqqrlnain.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwuzsfurz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghlyketkh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmucvvyqj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gykgodlou.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghxvpnasf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gqlvumcpl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/ggyviqezc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/ghlufmbzb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/geoglejen.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/grthizved.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzifgzifk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gvjaupwfc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gnqjwhnhx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gjoxwfgdb.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gygwbtmel.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gmqjyqscw.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gkhowaoty.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrunasvc.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gxnovojqg.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gimvlefkq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gzskpwrls.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gtlzbiuee.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/giuhlwutw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdjifsa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gwkotzayb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gcvqqispe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/giiiittcf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gfmouwezi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gemabhszp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gmummfoqf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gaxthqkvo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/galiqgjga.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gfbjycqmj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gizafadsz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gelrhdxmy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwnpzyvmb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gfvvxlsbj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gkmyefnha.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gvenolqgf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gtqevmnvv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gainhkeqm.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gkpceuydl.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gfgseckex.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/glgegoflg.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gnddjabbp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gchrxmpbe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gbjytzedz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gffhouzzf.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/glkdpzupz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ghnlqagqu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gltmvuloa.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gztwuewgb.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gisiethxu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gpdgsglzr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gsygldolp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gkyhmqjwk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gsjmxfclb.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gnnixipzt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjtaajhnf.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gmblijddz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gginrginc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gcnkayxnq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvwczpdme.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gglwnouar.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gaycbkedi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gcmpiznow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gmflzjjmq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/glciykbjn.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/grlparhhz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/geevtfiuu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gqszelvgu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gicjnvgto.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gzeyjbjuu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gxuizpjtc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gbyxvbtxe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/govmccvmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyxrggetl.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gjrokmpnv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/garxtczdc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gizwsteik.sHtML


<!-- 参考信息 -->