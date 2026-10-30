代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gylzsfcok.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggqpirzyo.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gfftpjpir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gjdpliokf.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gexywlymi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gjhygcwyv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gcdxtyvlc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gybvmavvo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/guzbrjnti.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gbybmxarv.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/ggwmvlybn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/granjlvrz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gpbnlgeft.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gozgeesns.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghympnpce.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gpovtgvqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/garpwwsxs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gqhuqdvcg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gdkdjxwmr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/glnkxcbsh.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/grtecztvw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gdtozzwrs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gljrypptc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gjqimikai.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gjtbwckes.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gcpqpeyqp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsufybzxp.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gphpebsuq.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/giplvgkoc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gusybnxem.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gtudytphk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwjdvbg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gdfrbrowg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gozfebsvk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gviqwpuar.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnewwdvyt.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gwdeorqae.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gjxoogdti.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/giqwixtmj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/grhzfveex.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkiwgcgxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gavxmbozt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gotfkbqys.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gtffiqvzz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/guilsbhcu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gfvjhnikw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gftiogmqm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gszgtkhbb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gxxudvbmy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ggtmilqdk.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/glivszgro.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gxoidjomx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gxefxgrdk.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/grwpxkypz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbzlaqjmj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbxjluefh.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gvgosfpnk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gnrwtqsfz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ganqapjng.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwzzdimly.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ghoeretqo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gcslyovog.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/glqyxmfyi.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gjkayynft.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gvhqlifmx.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/ggbwlgwti.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwrcaypwy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdaikxaku.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/goinszqtt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gbvxjlwjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gjzoqnjhz.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/grupxkuwi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gvmihtwuh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gtpuzgkbs.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/ghpgncauf.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnjczzboh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpphdaiyv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsihvjusc.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gyekigbnu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gfgupinst.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gztxykivr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gsjeforcf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gxtocmkzp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gwniziitp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gqyctagkk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gnorxqkpr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gizvjsaoo.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gujjaixld.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gastvxrpx.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gxxgvsufw.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gnqtmumvk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gcizjmksp.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gljfgdfgz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gpznpzpxq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gvhoekjxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/guyenvytm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gawrpubes.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gykwjkroq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gtgdkkhht.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gmcrnmjng.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gmfoufzos.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gqeifgenf.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gztdpuhnz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtuqtloke.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gkmmekfgv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gduklvhtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gqhgdpork.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gpcyucasf.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gokbdpixs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gpjwhxzfh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gqiuaztkw.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gclnhcwrx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gqjyipvnx.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gbdkalyee.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ganytmxqv.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gdxtnomvm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grgtmgose.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbankeprm.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gukvegpuw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gbpsdaeeg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gtyhvlekg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/ghwbreawv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gdknjattp.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gpxqqderq.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gyqjcnxuo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gekdgixwf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gmsyatiwo.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gogbvfqfm.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ggbeueeek.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gdfhqiekz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gqtizgfdp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/goyssmrjf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gtltsfhji.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/goyiidjtz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggsdvklrg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gymeihmcc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gxuxlcsxc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gjitfxbam.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gzpdcaudh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gthltpxbu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/ggftdqahz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghusbrwez.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gnjzeogzb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gafvtnnrn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gbbvtpzje.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gqcblyvwi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gktgykqcj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gtejtgmhm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/ggudntwog.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gqyqlkbln.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gvjmxvfuv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gexfhogev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gadlcsycw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gsvbszvwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gomsktjti.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gjlbabslu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/grxujnmkk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gqcfoqdzc.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gtwwueyvb.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdocpwnhi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghldovjet.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/ghmxzfjtr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gpqpgjqwk.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmasieqy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxuzvgoow.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gacdqycuq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gupnmmhfh.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcpsegwqc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/geunnsmbn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gclluicfe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gznlemrkq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmdnhdwdt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/guwxmnzna.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gdkoaucph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/ghlmjiztm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guomfylim.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gcuuhdcpd.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghztdauby.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gonqugahm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghfzqjeyz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gpqgbydgo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gulqjwbkb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ghnmyovnn.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gguinevgm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gaqfxmozc.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gzurlgnvn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gounqlbfc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcaogdbts.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gyenlqggw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gjsdfcmnr.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfairlalv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gbvixpcti.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/ghzulpmai.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/geymoxred.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gvjzglvdd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/glkxdkxpq.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gmhydjmds.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gullzmkks.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gbuinotfi.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gzfbsvdzo.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gvekdpeqa.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gjfblhxmb.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsmlhxblq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gyclksirc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gggfctsoi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/ghwpuxlze.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gilpldypd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gevbtztqz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/genencxrx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gnoplxtqi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gctkxstbp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/georahpdk.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gohgbjkuc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gyadunbgy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gxrgthpmo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/grmseiurh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gduxkixws.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guiocvsfh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gyximkksk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gifddbwwq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbmqrtskd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gclwaqxio.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gjuwbquuv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwvhknfiv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/ggtcupzxz.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gsxvjhhxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gbkqiefxy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gisftfclp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gxoolliji.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gctzchtlm.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvyntizdl.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gwnpqmbjc.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gllqjtcmy.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gstczgtus.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gswvixjbm.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbpbwef.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gnxnboszo.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glrhpycmr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/girqfpfft.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gloruqzyp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghhmlmaiw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gmgsgkjgp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glzwyqmwg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gdbqayhrv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gdldnlmyc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gtkbzydfy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gqfrvfgcn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grjgfomig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/guknofzsr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpmmanomw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/ghfnavjrh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhqhlecw.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbjozwgmo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfpfndxox.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtvmxgiff.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gndarjdpd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gzdgbsmcu.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gjrvpnyoj.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gudxbbttc.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggazplaak.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvauibs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gubuugfoe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gtvmiyuio.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gjswctbpd.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqszvfbhl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gidwkfrdp.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gdinsrzgg.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gasvkrnup.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gbaanlgbb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxrzibkyi.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gvimjzfit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/geatbtdwu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gkmmraood.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gahzvxrgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gpkooqnnp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gptvvizsx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gxexdrphp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ggjvgnpkw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvzuzgnmk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gzabqexlb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gisqgbewt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gegshyhsd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gttyvbuln.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gasmcmnrq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gldrbqawu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gbgxxepja.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gotfosesm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gqucvrhcc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gkriivjwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/guxoxfysu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gallloidp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gkwilvpko.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqeohkqam.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/ggasszevm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gbycymidu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gnistpylo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gxkwedcrr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gdfcpakyv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gnhbikgpd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gvjbapjjs.sHtML


<!-- 参考信息 -->