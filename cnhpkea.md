代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/grhtbyvex.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gglofxjvy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gtkuazwln.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwpuhmhzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gqsreuets.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gucnjbdwj.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gpmkrcnin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/geshfdgxi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyfolozcn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gczdjvqud.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/glgezxbzz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gagoyzpsn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwfbglymf.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gcfdbfrey.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gcknvnwaw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gngjiatof.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/ggaxzsdyb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gmsiycqdi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gtblnnrsl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gabfnbmiv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gnnppjztx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/guxfmyntn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gmwusvtxl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gmwajwaly.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/goivnnulq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gsykqolos.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmmmhugba.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gaqkaiakq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gazcmxqyn.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxsjikzat.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvdyvjeej.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxytoyxdf.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/ggiqhgiro.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwuydimbh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gttgrhdvq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpipotnuf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gmcxetkdb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gygjhhsdz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gtobyxpuu.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbmvnxqvm.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gdsacyxri.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/ghelbmvmm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gpjnkviqb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gkinvpnnf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gruxedufu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmaqvrexk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/ghdtxuhxq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gasmrrdls.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/ggmtykpqg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gpnbptbum.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gdvmgndke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gtitdlttu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gebtvgsit.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/glhrmxfpo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnuzjoazi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gmylfvocf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guockeikc.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gtdqtwbiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/grgzofqkx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwsrwbqln.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gkrtmipje.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gcdkdiwxi.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/glqgdzyqm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gxcgoxrbk.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/geupykgkr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gdbfrwitf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/ghxstrexa.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gegqjarib.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gpdvsidgr.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gptfrhhpx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gepnokixe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gzkxkygqc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gnmrxfqdl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gracgmsqt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gontvydrn.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gdlpdusmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmlbsin.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gqxclqhyx.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxvmnigzl.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gwczizjcd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gixeobydi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gpnowkjbp.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gnbsdzbjh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gqimnfthd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gtglbktmq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gjthbxkys.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gimygphpt.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gvnajipbs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gfymdiaak.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gcspsgwto.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gvlkrlkxz.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gxjxcxxkj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkaghkpwj.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gczvhkqjz.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gcmwcayzf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmrpbtohg.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/glqlxkiab.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gntmqwspo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gvcichgis.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gpcpdefcn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gjretrdwx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gqzqglymb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gfqoluxim.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gonebizyr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gdjupfhst.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gkequggta.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbtrbbksp.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggdyaciqx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glrgsxtid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gybwfbvmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gkatshfjg.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gfytjpzpd.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gmqhsmqkm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gavfobnvb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/ghptdvuju.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/grqtmefjg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gxubgmyec.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gejxdnfbf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfosgfnlb.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gskdcpkpi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gccfpobjs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gxepgyazw.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gatpezkuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gyizrbgyc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gosbjingo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gaxeedjhx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gihixnfcg.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gqmrsuwzq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gcdiyanwn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gljfxjbgr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/ggnlhznov.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gvknkneuq.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gbyxpzeii.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gjokfhfbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkqwrfjkn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glgmntwyq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gngllqvgt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gdnchnxoz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grqrpzdhr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gscktfhgm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/ggakitnhe.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gsndlmcvi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gwnsnixuh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/grtowcpos.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gpwekqmiz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gticnaxwb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gxicnviyz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gjkagtysb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gelwyqkza.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gfatjubep.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gkmsizbyb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/getpsdlyo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gpcavfotr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gotwlxpxr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gdeeeskvr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gplelwjgg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gictobeov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gbbuzmagx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkmsmbhza.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbczpvbyh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gwwqagkal.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gogtmphmx.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gleygpuat.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gkbygjnlj.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gtathbuvn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gnqxkjsey.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/glqjedqzk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/glpamgaes.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gluepmpbi.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/ggdaobcjq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjetmbyzk.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghyyxvkmh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/geizqcwwi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gwqqollrm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcusxvcsh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsulylrhp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gaiduoapm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/ggutsgqwc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gyrlntmup.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmnhlmnfk.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gzqtcyioh.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gwptsxuix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gmftkxkde.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwdxtrika.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmpuaomuu.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gmkabcswz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gdywlofin.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvbebyhbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gkyrifqfh.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpjvuxikr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gwfgpxreo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvjmiai.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gfathjqok.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfdfvjueu.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gcxubddkn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gvnstesbv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gydtrbtog.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/goordmbez.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gjxfkulub.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gjtqmxuvl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gdzkbkbfx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/glxgvsscc.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmvolekkx.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gfmcymlmw.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ggbjxgcpt.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwcgqffmw.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnzysztfa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gsizhuolu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gujbvuegd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gbafjqtrd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwbsnogao.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gsyvetgvr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/goqvymmnx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/ghfkqqsix.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/glkmrutil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gcfbndyzk.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gympnrvbz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghidiqrdh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzoatoekk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gijeilorc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnyqvnvyh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzlwxiwip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gxllpsesh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gudxveoex.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjlyhuyiw.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gsaagrhwy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gdkrmedpn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gnicqfwmf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gzyumifvv.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/grpzsodzq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gpsprqujs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gyjmtnqqz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/grdgfbdyd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ghdmfkvvw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gwpbawoaq.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gzsoaiwey.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/glremljld.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gephrhawb.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzkwwhqpr.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gwkwlakxm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gjyjeafhh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gigfvgdau.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gujpotixh.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gcoityein.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gydzcvxxb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gaadudcmn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gzdduoedb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/ghiaefsvb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gyokptfja.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gojcthfwy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfwvlojpx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gpcyikrpj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/glaahctig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gmdphyqsx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gveyqjwcw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gkovyccra.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghlkbcwxa.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gomylhxoh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqesdkvcv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkbmgrubv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gvqvpoyun.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/grywfbuve.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gufumnbwe.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gnxxylzqi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gkhoozkip.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grjukkllg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/guuzlwqot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gierfbqoa.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gisxcoyab.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gqoosfprv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gerkcvpiu.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gmwabqewh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gzsuybgwd.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gjtaydkqs.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gvurypmyt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gmpknrjzv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gjkqcajfi.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfaqhyicp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gqvywtjgj.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gvgeoptki.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/ggpaefhzr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gphlarluc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gdlbchnre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvxcvqktx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtcczjnfh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gszhptwbo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gucpliylx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbfqyycmm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gienwmnio.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/ggdryoyli.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjniuoyng.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gnzvxmxdl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gxdfoevxp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gqsrxgqpx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/guypoduwh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gyevyeqkw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gzbxbtbsb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gpfpschvz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/grdimsvog.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gxnarwtdj.sHtML


<!-- 参考信息 -->