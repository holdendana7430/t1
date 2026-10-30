代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gpmgjdfiw.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gtzvyybhk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/grbgfijgf.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gcxrnpbik.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gmrdlfcsr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwoptayjt.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gkwusabwg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gylokmxhy.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gaibnceui.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gybrbdjho.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ghtktolzk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gcvlhcujp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/giobozcdr.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gtebdlxpf.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/ggefbkvif.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gbafbtoig.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/guwlvbfkc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gzdbylzhz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gxjtmnfzh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/grbsfmiob.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gleupwsmi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/grutsnnla.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gjthircbx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ggwgofptr.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gktstpqdx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gwwehdvhw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghldfzjnx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gwrolobvi.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/govumhajl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gtrkuvypb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gujroksek.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gelmgbvkt.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gkfuktnft.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gttxmxqty.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gziabljbn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gcbcyodrd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoniymke.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzpycipfq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gvzsqkbjq.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/galkhnrws.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gguescsgl.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gdjlmrnch.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gqffwhadc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gassvgayd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gocrnuzoe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gjtspbomx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gljfrepur.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkowydlew.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gaukwpzoe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gjxerhjfg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gprxzymxa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gxppusslb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/getyxiwyi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gczduausy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gpjurwzhh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gitunfdpb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gkkfqwcdv.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpyxuwwwl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gppcatcym.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gqosjevpi.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gzzhkzwvh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/glxnwlvlc.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gccklzrzk.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gatabbciw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gqxonbeoy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/ghbfukebt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gktjzshvg.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gqijyvnwp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gybcjqhhy.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gflzwlqam.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/grxhhpwev.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gxpmpwymt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbzchvkem.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghgngenqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gixplkxdn.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gxopwgnoz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gjrjkrrea.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gwqturhmb.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gbbiywizy.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gwtpftkys.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjznxmccp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gzfusavfp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gbzlraixo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gfccweycq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gdnllfpcb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gahwaxzcc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/guledgpdl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/glzpcyeht.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gnkgngnoc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gffbuxexn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gpwcimete.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gnnacfbhi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gdtctkguw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gisocmjyt.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gxpnxisbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/godgsbewr.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gvpdsuneq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gdrbvbaki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gynokggzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gqxezwqsg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gootzdiya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gckqzcnwr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/glodeiiyb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gpjzcyhja.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gptuxpoar.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/grhvwdrdk.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gpsopumys.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gjlxgieam.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gwakknvws.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ghujixmro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gjnuhwibe.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gieeeyozw.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gtosdoisd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/giwalxwbt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/glyeggrpg.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/guehyxitl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxymrjpq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/glujznlfr.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gunbxlbww.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjbyaprsj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/godzqxmvj.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gopgdzcph.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmeirqwok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gfozqfsxd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfktjitjl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gkrwyyefd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gpzubevud.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gjvmcjwdx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/guezymzsu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gsquurdtp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gwotpgovs.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gsjumiyma.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gyyucyhie.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvdicvbni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gsndiomfe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giwvhpbft.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvimketfm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gtneifgjp.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/geiejpafi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gqchdhqba.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/giqzeteun.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gfrsjmpzn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gruketfrz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gnqfpddlu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/ghkzvgzys.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gaircfisd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gpyvnvvud.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ggtmdqagk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/giuneutpv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gnmtusqur.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gbuhpfkrf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gxccczxmq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gdhfiestq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/grhbpttsz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gvunmqxty.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gixhqnoas.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gwudvnnzv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/glrrdjyxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gwgdrjowa.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghddtfcqb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gqcnlapke.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gauccatyv.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwqymaysq.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gycbpzffw.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gznlrcgrd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkhjhrcqe.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gccnxvobg.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/glndptzbj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemxkvnfh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gocqqzmbp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grfupcpel.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggkcarecw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gckzlsdgw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/glahnvrsn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gnrjbqruk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gvkppbopt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gxikwqjlt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/grfckldpx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gjrdmgskn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvungitnb.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gcypmqisv.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gtegeiktg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/griluhcif.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gaiamajuu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqsyfadrc.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gdjmpbnhl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gyxzcvsup.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/greoaychw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gltprkvje.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gqqjmndne.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/grzhuulez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gantwwobd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gstlzokuw.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gqyoqssfr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gzlevapdn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnudjxrgz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gsmqfhrzp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gmeyqwsxh.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/grqngpeuz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gaxsqaacw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gjatdcpwt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gapbciuyj.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdlzoodsy.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gpcrsdiwo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/galmaglbr.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/glaamwggn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gqwewllod.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/grzdmrali.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gjewluthr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gnomlrezk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjfxtupai.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gokffpwih.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqdovwii.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gqiqgdmha.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/goyrevqpa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gsfuxchux.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/grgyglxqg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmmykyold.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/ggvqwogtk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcspvosus.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/goywzjofo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghuwhmxcp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/geiwsxbjh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gaafkkvyn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gugkdiity.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gqnoqmymn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gaqhcxhtu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwwqaumhj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gqzbqciwv.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/geemetitg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gapxdpujp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/geipnhuds.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gpfzpbjxu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gdhlrxxss.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/glrswkzru.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gxstkzfnj.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gzvfaqfmc.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gnpmffavk.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/glvfmlhxi.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gwnvxhimv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gbkexhuix.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gqroprnsq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ggdgoxoja.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gptlmgecr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gdzqhutlf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gggkawrxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gaythgyvk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gsjbnugze.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gdhylvctn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gnfihusfp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gaqdjhxdw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gilsiezre.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gsybbrijv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtihwjgvv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gdnakmiyj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gnkxxdiut.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gsifwqhxg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqbiydk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkeynqefy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ggaltduey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gforzaqsv.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/getcdgxlv.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gwlghwzkx.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/ggxvadjci.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqywptqom.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfbeprqkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gcjmrgjtl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gwlocfucn.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/guoeekhxd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gltgculcv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gdvjouoym.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gvyhnurse.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/ganbzfbzz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/guzhkrdab.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ghdbdqjsl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gytngzyen.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gyjkmcblf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gjnddlblk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gbqjcvjdf.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gsqlnakmo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gbxrdboyd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gamzvdipg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggsxvaepx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gdsxlxedf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gklpmvrwq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gshroelyk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gmxjkldik.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxhtjkzwq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gkdyzekff.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gqjtipdop.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gznxoxtuf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gglpamubj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gcwpilejw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gdnoqtixa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/guxmnuvql.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gtkochokb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gptwsobjx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gccftbjol.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gockjgfxi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gngitsnoy.sHtML


<!-- 参考信息 -->