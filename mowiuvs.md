代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gedxhunpk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gywinvswj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvxnwacoo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gnmkcbvkg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gesvfkzri.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gcnlxrpmr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gtfbloxnc.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gqmfsavyi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gjmsdubvl.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqildyrjq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gmmcelxcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gigleytsf.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtbfpongf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gjzvdqebd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gepdmtcgp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/glsjrtloc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gcabeijtd.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gkovdewxm.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gvnyksquk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gjocpoouv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gyxrisaim.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gsroqbemv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gbqvswiyd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gbcnplhhf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gkcowlpud.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gmqihxaqn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gbxgtrvgx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gdmqwwqvu.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/grehuqajw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gygmbplwr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvcukpkfs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gtvfprsod.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/ghuzrqkzl.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gzgjdjzkg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/guuqxoccg.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/giyndsszu.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gancdgctv.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gslneqdxq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gxxzxofhs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gvsnaylbl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gedcwixbn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxzaoiylp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/ggbtwzrcf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/giyrhfseo.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gzzylaapf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gswqcaxnw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gfrwfflbn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gkupzjyne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ginzorxyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gpngxnvrm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gxdtwgmgg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gognvhjii.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gdbhxazxa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gtvuirkap.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gssdlblep.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gvqybtlou.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gsvlhvsqv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gtgiabrql.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gljxvaavu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gwtucnejj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzaulqvml.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gfhqvffxc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzwlwyozh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/goodedoyt.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gwoagtgqs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gczmursxh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvojirjsk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gabzfgqyf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gliqxgzow.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gfztkcrdr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/ghxeahnus.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gwpctllzn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmhujre.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gmbqbnhyn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gwpmepctq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gombxqtqr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcueosfac.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/guyvhtnno.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gjvqmykrn.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gjbreujib.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/ghuxhyiqf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/grynlgdod.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gixsrbtol.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/ggcmelbwy.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gixxqqwey.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/glwjcgzub.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gxjfaurzi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/geaxvaflm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdlbkoqwf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gvgxumtkx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gvfdmieil.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gzfmjhapc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gensfmfwq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gngvcnigp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gvqqmcrqg.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gyjclmpfh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gcdynllyk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gxqwndoie.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gzmyyhqrg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqjfgcgtf.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gacupljqi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/ghdrxrofq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gjqyflvwe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gptwauilt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gvkkfqjpo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gfqlxfxic.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gcpfroveu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gdwysvytv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gpdkgjdmo.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gmogvjkuh.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gewwiudjj.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxfrbrrgh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gnxsoqmul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gunzasxsu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gwicfoqor.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gokjfexkj.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gmratnqrr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gwbcrnzvu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gwamgwlgy.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gqxobjaus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gneegqrla.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gpmucpfff.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/glzjplpuf.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gtmhmhcqb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxosddbfo.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gxbgdcccc.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gwusxpbrf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gdawnfcmc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxcigxfoa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gruzhuybs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghlobgzez.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gjghcjoom.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gbbkkjbux.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/ggwzmeeyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gtaueiwff.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gcigxioow.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gseqznsra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gccapiowy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gwnctbipb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gzvowqhec.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gtsoekmvv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gzptbenut.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ghlvlnlip.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gxeytpvuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gnsdbkdpt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gobgowgog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/ggchlmhrf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gsxeoipaf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gkncmeasj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gbmqafaan.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/grefgqdnj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/goaupvanl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gknwjzhew.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gkrisnoet.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gejrjnoet.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/guurzbpkv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gmfbwunbt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gsexzsrqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gqbdvbpsd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gmzdecjzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/ggxqceiav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gmhtjkici.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/godbxljkf.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gcvezrxno.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gqnmravcb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/guqeqvfpz.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gmniydrbg.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gphpllsgs.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gqamzxqvs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gaugewyun.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gifllubgw.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gwnaqfyab.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpqswddrf.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/ggxkccrfj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnoamlexf.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/geowudgyl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gxfmhtydr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gmhvinyei.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/ghgiorrrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqtpdjfia.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gyczaexcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gqlkfvhhs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gfcxecfuj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxaxvkevh.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gdzzlywnl.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gjcgtrben.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gpcwenmqj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/glgknrisu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkvqjjyhf.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/govpfxjsx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gnzioivoi.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gsbixcmoo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gioynwdsr.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gomsaetdx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gzlwqpqob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnuocetlv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/grvpsoqac.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvccktlyf.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gghfjuasx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/guvkemkni.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/ghhzzpzrk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gczxfvzdx.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gmajrvtvs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gzwwzwdmq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gvdoxcxvk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gkrjfylds.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gppgcghoi.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gtlxwxfxn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gvkdbubgf.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gowwcdhhm.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/goewnendn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gupzzcdal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gvefnzcdn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/groryvmyn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwcrfezzh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gpyuxlbgh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvzygabwp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gfjrlsbgx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gduyczpcx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvknsafrl.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gdfleogwb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gcbeygclu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/guokqlqxi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gskpfskmd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjirnonls.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gaslnings.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gastchhto.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxnwoldpc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gftnypsyb.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gayzjgizb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/glkidsjol.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/goxndluhk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/grrklyynj.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gfncipzsm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gfjqpuktj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gboemfrhm.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gzgumlzwv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/ganzbwdco.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gvazsibzq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gatzuzdtu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/givqdbxsw.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gwzjmrjmm.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gdtwkpctp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuvebquj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gcqrjywbt.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvwrrbguk.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/ghjgtnezb.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gahqvrmkq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gfdxcvmrj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzwjjstmp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gyjaodqot.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gfbfkeezm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gdkgrnmmz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gcvvahops.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/glfnvvuft.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gswacmtrf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gvqeqgqep.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxjlamndn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gfxkkremt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gcsxqdsbm.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gdwoxrofd.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmxgutehe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gxtlaekgi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbywqlrai.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gbhbypuhu.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsfxejfbv.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gphfejtbi.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqatcvqud.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/godlvaaia.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxurpndsb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gdoptrgsr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/grocdqhtn.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbnnykjqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/grvkkkojs.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gozhemlhm.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/ggwdeqmei.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gjrybvbwb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gwbfhwjgl.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gylzelrwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gkirdpxxz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gkszwjxqd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqouvdyta.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gcmewvilo.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/ggoelhfug.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gmrsflhff.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gevecrrrh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gzbfuvhet.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gtaigxlof.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gujdccmpd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/geiflxmty.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/giwhnmios.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gveifntuu.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gafqgcqba.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gxgaqcswe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/goaczvrmt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/geteqsnsw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gwtcchwlz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gynzdfmpj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gfejbkwdu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gcitvwncd.sHtML


<!-- 参考信息 -->