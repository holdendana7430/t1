代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gzxtsomhv.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gdotzftfj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwgzdnzi.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gfrhytlvj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gnyshybwe.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gzbynrwuw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gerblbjrv.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/grhukhkna.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gseehpuex.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/ghaylgesi.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gnlfzzfsm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gebbrjchg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gabojdmlm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gkzywpafu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gaifcfqnl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gvhnfkwop.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnxktnwch.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gcvdaylnm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjrzigisx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gakndxpzy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gsgsazoay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gizmfxgzc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gbjfmhzin.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gtuulnapb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/ggkfvgrix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gqpbzwvyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gyrodnmma.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gpxzmpyqp.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gjwrjncpc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gntpegaeu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggmaqqbez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gponklfms.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gszhhsjtl.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gybqxttwp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gseongyyq.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gpcmzxotn.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gyyjfwaoq.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gajnheuwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gnzgagodk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gqdtlbbcd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glaufwqvq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gravxwvow.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gojimerad.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpgmyldqw.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/godngwsrq.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gzcnipvps.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gjuvwldqx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmjfnzfpe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gaqfsqlwq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmfpeiqrc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/grnkbnpcz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gtagubssw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gjrruzusw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gggfbikyg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gluhnabvy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gbdrrzrrr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gtraaldta.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gbmrzpurf.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gmjpreach.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gcrotrmob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gqwjfymzb.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gpahwnblz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdhczwnzu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkwscbmyk.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gvelihqbp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gnokjaznq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/grxqxunlb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvvbtoklw.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gwrxlaxnr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gcozgqedn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gmgleajoi.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/grbhoesix.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gdfzuvkbu.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/ggvbedcvr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/grndblhte.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwuldqofm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdatpxakm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gokwejbra.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/grjzsifzc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqweljumd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/grxjcybvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gsfbrtecn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gpdrgekbn.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gtnvtbapn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbyzpqmb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gvqmxkjsz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/glaglczkf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gofsbstht.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gubahmtkb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/glokzvpzr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gvhvxpdcg.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gffryiiwh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gqkifleyr.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gqeughppu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gyzdpifwq.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gvepldfsz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gljivgnbp.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/goksmpwyo.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gxazpdvni.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvwdvfyzs.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gqcmjnsxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gwpbsjxgq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/grovuctde.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gxvdhwuek.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnkpuyhaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gqafnekgd.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gwdpkptem.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gammdcskm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gxyxhoaps.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gexopkkvc.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmqwfybzh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ghuottypr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpqomcski.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ggcskabzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gfnpunzvs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gagryhitq.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gkjyksomn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gifhaepqb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gqgyoxvws.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gixsexvgs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geidseodj.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gupahyeyf.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmporofew.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gikyaeyth.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmngzndni.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzfqneemj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guoadtoto.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gnqvtxhzr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmwbykylk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gslgubeyp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjfwieg.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gmusffxrq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gewupwdvy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/geflkjwob.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gdaiboevz.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gvyctvjcn.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gqsckyvtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmkfgza.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gfshicdhx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvxcytdvq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gmtbrxwxs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/ghefuqqvj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gmucrnlfy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gtdegmzrt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gknangzzj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gpicthkjx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gdlrkjxhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gxlkgmswd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gqlineior.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/goinyfrti.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gfrhprvkx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gqyzykujv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gbxkdxtgk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gvopezosu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gcoslprvv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gmebhfkfx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/guazrbkqo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gkwvjqmrj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/ggbhcblam.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/ghryqgjxq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ggviqcppq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnsxtgfif.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzhrvagmd.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gclsyulhr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmjdftmsz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gqndlleha.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggtiktlmw.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfcbpujpj.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gtycsjark.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gyqmruagd.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gzcsjfwnj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gxgsvzgjg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghgamusit.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gvtoyqhkr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgacxyvb.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gygobokcs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gqjdvykxq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gunzeacqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gqseqltjf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gzklbzqra.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gowbvuxkj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/glecwueol.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/glwtjgcgb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/golloxsfj.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gdcdknorj.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gjqexxzqw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gzuokmtki.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gernxwmsv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzphcwwsb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gqfifxgzs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gtpwvgbpn.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gleprzdtc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gboinwypd.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gnppeqbnw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gbkjswceq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gorlvbnaf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gifmizvmn.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqwhvwuab.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gamushrfn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ghftgdyul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/goevgksnh.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/ghqaronid.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gimkswozu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gjyvsgqmb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gmlerimwy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gpsknirci.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gasokndvw.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdvzgkvcp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/glfkcborg.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gydcfhosm.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gyudqaule.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/ghsksfeux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/ggotzwuql.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/ghvbeivta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gmfzbpcox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gqewywvfu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gekdoqzld.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gbpbgdvpt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gnbofwkbp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gkyyapcfs.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdklaijfd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gbhispezr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gtmukotfc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqxsofcat.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grwkdaufp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfqophprl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gjfuzgocn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbhuseobn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/glpisdxgb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gjgwubddo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gakgcsrck.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gqjujjztq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/guemesbrv.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gwzbzxpgz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gdmxlqrhe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gkamimiit.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gshzlskuf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gshvibsdh.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gqrwdkslh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/grpfwvjzp.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/guflfmrvz.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gynfnhfgo.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsjnafgpy.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwwvcghka.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gxfyngtme.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqypwekvr.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gsvsujpxi.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/ghvxbczyg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gatqdxrga.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gjkmxnynh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gpjilgqwd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvvzbkdok.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/grioyshgp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gswfmjxok.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gspqpgesd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/goiuyatbf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/glesgilsk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmaslvqfr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gxzfwwqns.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/ggtmgqjnf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gddzasnqb.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfmonkxlw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gjbdmbrvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gtveqrpjq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/guwbooevl.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gccyuvsag.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/guvhrxllj.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gyxdxticq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvqcvyfmb.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ggwgyawat.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gqxyvcezw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gberwdnsc.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gmhlrpzyn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gphwkhiok.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gfqjastmb.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/guheduhti.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gaotihaxm.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gdbknrori.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gigcsllrd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gmonqubei.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gwdhodblw.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gibfvihao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gyonsnbce.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gnrfhosrw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gbiozaamb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/giobrptca.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gkdwaczgk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/giysejrck.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/glazfcnpt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/grkhmetgd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gbxcnkcdo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/guwhlpexb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gfbkyypri.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gnkbooihg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gldcozwar.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gpecwzqay.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/grzmbhyhc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/giwqbvqzx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvxwsesuc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gzlxzuail.sHtML


<!-- 参考信息 -->