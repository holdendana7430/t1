代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqedtebai.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gqvkwiusv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gkeuqyvqo.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gxhvkvpos.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdkmcghqe.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtliasyyf.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gvkvzirkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gqeviyqvs.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/glvtphjrr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/ghhxauiya.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gbiyxtnph.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gotxemmmp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gazbaaxrh.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gouzhvkpq.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gjmhsforq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gzsqsfvfu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gmjrxohdp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gnfnhutao.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gpuilbgui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gwdsmmfns.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/geexgsbej.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/galrcidfz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/glpcjvgxm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/glzufxxcs.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gigqagwoi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gkcbodobl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmssyxnsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gwsazczys.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/ggmdzlyzw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/geiyalxtu.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/guiplxzwl.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gccqzvvpn.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gtvfxbwqi.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/grqopbmwf.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gmfjyilza.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gcgmtxpnc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghplvqrpc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gauwpswlx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gidqkmxdn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwpthbzuv.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gkvbjkmpz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gwetebeez.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gypiawaum.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/guspoidcp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gehdvohwk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/geifakjpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gicpldhjz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjsywntae.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/geegzdgon.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/ghqyraiax.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gziabnuhw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gshqhawyi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/golmcgizx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwnujbsqg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gizccunuw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gfwwwtmzc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gaqitiqmn.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gflcffcdb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/guzyfiypa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/glvjqsipd.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gtimtyxac.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gngeyxpwj.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gesevvisl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gygtjmuqm.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gxpzqflxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gaccxedzx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gdngovcwo.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gboctjebl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gooxixxdz.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gugdownpa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/govywumdb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gdshbxjwe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ggxzlqyfg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gjtkfbyfw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gcwthgczb.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gefjmekqt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gclgyfmhe.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gbgfrsqon.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gffhpkuru.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gwhpspaem.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giwlnvhir.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gxjcqpxlj.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/goazfgdzh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gnjmxwdlo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/guhxnffzr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gwkxcaoqt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gmxyrtiet.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/goyuroymd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gwlbqupnr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gkbolpywq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gpvirenue.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gzzouwjkg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwewfqylp.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/glqnyrdqu.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gafvohofu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/geukyrsem.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gnbovmrcz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggjipisrt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gfhdfoaaz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gsavgvqax.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gfdgluqts.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gwlxybavy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gdrpjeqql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gcnragnwp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gdfygusvb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnboifccn.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gnrcrdbdh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfhkxvcal.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gbcxvqivv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gytmjiljs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/giimiideu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gdvjryjuy.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gsnxqkswh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gbcylqgco.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gcixleten.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gyivdmepv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gjeegnriq.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gchxmscbk.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/ggvzaqjrh.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gcgezfjeq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxqvaxfgr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gavlsnygo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtaaspybt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gdfkjwipo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxidqbukj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gyodaokqi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/glirnmcit.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnyglitws.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gdcvrvufc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gyyhswszu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gjblawcfe.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/grhksvdej.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/glwgvpnbn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdlliyemw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gigwhtufm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gosaslbfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gaafkebql.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gwyhkdnwu.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gimksegwg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/grshkhzex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gquatfaqd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gklucnnuj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gcgeoroqm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/ghnxckwwz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gscytppvv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gswwxxvxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gccduzrsf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/ghgrsajlh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gefznkwsn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gwytxzuzf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/giywvttxo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gdncfoxso.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gyvfnlcrg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbopbps.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gjroyfhou.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gtlmemzqv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gxxcljpon.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gpjmhueqi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gysyuohfi.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gzsvfpjbq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gzkkmqmpq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmpanwpxd.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnrsrhyyo.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnayfwvwy.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtzzvxnmn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gblluzopd.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gpfzsxivx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gsqvstbms.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnjtapqzr.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gjrosdbgi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdyqdvqmk.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqkmlhwtd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gcuwgvwfk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/godktfqhe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gmiakuzqq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gspptkfbo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gppzgatel.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ggkbiplqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gsdeafxxt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbiaebtkh.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gexuczzwe.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gquwtuedf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbywfsixl.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gppjudxml.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/guxetnigz.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzejwoduz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gebptsgtu.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gjgwgcmdd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzyguodev.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gcpnbbdhb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/giclgfmbc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gymfttrnv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuywwsoe.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ghlvxheyc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpjiimikm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/ghusymkph.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/goaoisuus.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gehemcccx.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gogdkvchf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gzargozci.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gnzzmztfn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gjeyedxgv.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggylygpuc.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmueiqyas.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/galdzcyjy.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdairirhs.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gypywydev.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gtkyapanq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gxgcozlmu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gaalzleqc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxbwepkuo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gwrzovdjt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/grkyabvig.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gyaxbblyt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/ghuoyvooy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxkdgwvfs.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gmolaxyqi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gbntoqzkn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gunlzbclb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmazdbyqv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gubmqoexs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghwaqalkt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gblhnmfpv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsooubnad.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfluuegwq.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gbnqwtqgr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gspfngirs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gzyjbgexr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gxndbygrp.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/geycqwakc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gcyhtblgt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjmpzljs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/grudiuedx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/goawcjthf.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gldyyxgml.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gotvnorme.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gemisyaen.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gktrlrklu.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gebdqehjw.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gimbycvgl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/ggquknnrf.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gxgcxjoab.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gafdcydwu.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gzpydsnxt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gatnamdvo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpcftoisg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gkotohdjl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gnzowzjms.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gcgimtgmq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzxzyzti.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gwjtemite.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gzdqhfgvr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/goflydfmy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gtitrsfkj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gnoqphhbh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ggefnybej.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnhhpuhvr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxsgnasyw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gwlypsrgr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcqayanmh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gtlttdeqq.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gpddxetfy.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gjehcpkkq.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/girdqfpdr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpzlxdwhm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/geogpotvy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbsflihnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gxgzhvsbv.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfbbvqmip.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gnaphkjdp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gfvgwkeax.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/glorazxwe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/ggdskczlh.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gyufinyuf.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gcxukecyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/grdycntes.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gfztphjpe.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/grhnjawdt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/grnevbsxh.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmetepgrq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/geixhhtbm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/grngmnnfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gaaumjswp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gyyrlcbzl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gszvfmuey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/govivwpcc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gdxhreqcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gjklqfjdc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gzxvpxnmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/ghvvnyryi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gfanuqvrq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gbebrqhcu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gbgkrpxsx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gcwecnqcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gsijwnnjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gcbfpfomg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gfjlgdfrn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gamzcwdiy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gggspxwpc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gdkwkuzje.sHtML


<!-- 参考信息 -->