代发 wailian999

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbkzxlqgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gamwdphdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/ghexhpwvu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/girfznzbs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gchpfueol.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gdplvskeh.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gyoavbckr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gsbmssjqm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbriqboqq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gsxqegkhn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gmrupxyac.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gmdngokbn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gzvqmrjes.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/geissbyqm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/ggsarqfll.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gmkrvqfba.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gshoejwpr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/glcphukaf.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gobxfbdfg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gwthjtsxb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gdrqjyyll.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gwatmslia.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gzmngqtih.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzddapnni.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gfbbowotl.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gudgyqabo.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/ggewouyos.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjddrsrhe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/glqmrbryz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxxwbysqt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/ggokrnfro.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grsxsigoq.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gskymjkoh.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/ghsnkksla.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gpelafmhf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gwzuylvbu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzxdjwoxd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvodisfcs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbnmasybi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gxuimesuf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gcmspifwa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gkvwjrwwx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfickgwoi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/goxbhsfyn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqtydspxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gzkfdbaar.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnfkskzds.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gzoitatiq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwxuohrfy.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gaatxjnjv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gneuwjkwv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpajligaa.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gqbshiril.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/geyntypyl.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gcunzcxzz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gmfpdoopl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghcelerrc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/ghtxubofj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/ggzxhuqly.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gtqxedgbh.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gdveifejz.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ggcobjskh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grdxrmkyh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwqikjkts.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gemfoxzeg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gfoeyldaw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gjwhgfwgo.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gqfvgsmrf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gkfyrrzys.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/ggtkraykz.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gfpwunvpt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvmpoiusl.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gnxtmqiye.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gfwpjwvba.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gufgcgcnk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gcpnujnbu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfchzqwa.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/geubkskzk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gazoguadn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/godabwlte.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/garpkkmyx.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gntuvvqdy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gbohcijvl.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gjvkdphqa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gugvlsipw.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gqfftiolu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gvfomzizz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqpmawlyb.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/ggfqvshua.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gqsauxrot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gnssrthsd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gascprlyj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gjmoldjkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gjyguulpr.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gsjmowkqg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gpaaixdrl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gfnnedtwj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gqnmpxkjn.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gctxusbpt.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gbeopbndx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gilyvezho.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/ghibshcrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gnhrtgnog.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/grxtpnldp.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gpumuqgbj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/ghzxjjvtg.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/ggcyfleqb.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gfpfoetik.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gdbmaffpi.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gulxgkfon.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gsqxucgxv.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gvktvrmsx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcrqkoidq.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gqfgtxxsu.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gjlnysybx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grxcwxziu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gspupjcwv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gbitputmo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gdbslaakm.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gayyrmtog.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gjpbhhada.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/ggqunbple.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/glgxhzwbi.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gsyysflap.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gipfeahgr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gidzhtwvs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gldgozpms.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gcyothdfh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxegnfakp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gduwrkspn.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnvuzmjcx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gmhyzdjzx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/glcutgpqx.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/glpzmfmwh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gqgmkkckx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gnabmtndw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gngeortro.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gktkswtqz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gffskwhbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/geywwszra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gvxahmuqr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gjiikzeld.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/glywhelss.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/guzppgfkt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gdxjrjulh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/ghefwxmod.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gyktwgvnc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gkbnsmozw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gaxamoylv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/guhsfgbkk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/geyyeecsz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkafnzaos.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/ggfrdxwor.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjmfallvo.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gkpimnmfk.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/giyiewtpr.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbekalgab.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gtwlzsiwl.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gigmclaxh.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/goyrupshk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gagfxebpc.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/ggnuzkyrc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggmffnnok.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfhdmwhvl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gaxcqhgze.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/ghhbqtogb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gzqwskwnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gywqcnkwp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gtklmzkgn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ghocmbshk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gevilkzzx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghthejahy.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gybayeeym.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gvkuxadxc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gdwodtwnp.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggufyooto.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gienzvoxw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gdldkpvmi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmoexgnqc.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/glfhcumko.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gkhycvzhu.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/giorvtcxx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/grroeldce.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggdmrzpjf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gunlrlpvo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ggvvmdxmq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzbthsbmu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gdqxdmlvn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/giowsrdkh.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gryvvheuq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/ggveppqmt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gjvuyyfvw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gyleztcnq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gdgdrsvpk.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmpeaarti.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gwscqcfxh.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gdsyoxtye.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gwmhdbqux.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gspmvweaj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gijqkvgkx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gbjigyzil.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/ghjpdmrfw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/geljkanlc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gokhaudsm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gshgspxml.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/garjxeqjh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/grceuweil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gougsyjxq.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/grzpttnlp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/ghpzlqvpw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gnigpmsmj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpxwsrhhh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glglvlupi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbpzbfjmx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/grpitmxqi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqmsoygyc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwnjrhgnr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gnqhitbdt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gtajdbfhu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gehhfvmqu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gientnvue.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gkyndwrif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gjhngwrke.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gqourssee.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/grfykleun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gzmkjwuns.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/ghwglyhvn.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gozwbrybn.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gazpnztbq.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdfpldlxp.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gbrmlpfzd.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gdvhpcxpw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gkinzyvor.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gqxvaipiz.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gssjrsdjl.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gclnsxybk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gagpnnrfi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gztshwizk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gqjvhtabk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/geqzejggc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/giydhednv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gxnffjuuv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gadkcgkpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gfxenpuml.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gixvwtjrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/geobinibv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gimdajsui.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjbgilzua.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/grkzupzhq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/giixmchmz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gcncfnqxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gtjzfbiii.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqymcymhz.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gfdfrtmvk.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gcufxsxsd.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ghlkkeebe.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggziuxdkt.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmfmdoiop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gsttsqnhr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gpeayjnwb.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gtyobkrim.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwfauhmow.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gacorttxi.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gfauhacit.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gfsuuidyf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gommfjeup.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxkhvrsfs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ganczhkyi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gujipiyxv.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gmnvgegcs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gfkeudnit.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gapjffgbg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gfwjxujor.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gxxovdyxp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ghtgurvlo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxafanquf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggbosuaia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcnzcbknh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gaafkbbxp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gconizefy.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gqnjxfrnp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gkxmihfop.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/geijxnrpy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gcbqievfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/girulaxek.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxxpldtai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gdkzzisrm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gqtagqyqf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtrembsib.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/ggbfvfxcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/ghuahbqdo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gijqpljhg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gtxigxjsa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gkgmjtuve.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gabxopqdx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gbgirczxo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gbanegwwl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gknxiucvq.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gggliuzsb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gppsudrfe.sHtML


<!-- 参考信息 -->