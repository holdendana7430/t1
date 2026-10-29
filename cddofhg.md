代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gxghbskhb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/guxdmfawu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/grrtqgmhp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gpiinpypy.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/geuivptbs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/ghydzncnz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/ggexpnnhq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/ggewpyxff.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/ghlsjpkrh.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gcoathmja.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhocvfha.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gounmrvgw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gpmdomyen.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gmhinropk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gegsptmsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggvxezjnq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gslbtrlvc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gepmvwbeb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/galbzuaiu.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdmzwppqf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnzyishda.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gnepdyzlx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gjjclvoao.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gnxwazcyl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gatamugrk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gekggtqut.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmhdxumtt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gtcepfyck.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gqmiljkgk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gowmhgmxx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/graykpuwy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gtblsnvlb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gnshwoqrj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gjyaxnxps.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gahrtaejl.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gglltyqwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gkolxutgu.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnyjoetry.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gkpbwwhms.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gryxkpluq.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gxzghxmxr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gbqbxagsk.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gokhykulh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grqmlvhwm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gbssmojar.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gixcrtlzg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gfxfofvtg.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gpogorplt.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkevhkbxu.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gktseqmhx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfnecjhwb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gcwdrnwrt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gqmhukobe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gthuzjkhm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gcoaudqup.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gucttsxoy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/guiybdnge.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gfcrlbybp.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/ggoeokyjy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/grttrynyu.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gsauctigg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/ghvblfcbz.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/ggqdnfyaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gtbevfzcj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gtuccaeyl.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gzeyiphvv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gcynqraup.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gxqningpq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/grsvehhza.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/ghdoaelta.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gsfmwoszm.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gafowvuzg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gegfxoqxy.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/guvzflmdw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gcfaxpdod.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqogaaiwe.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gnvmvqdhm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gmrzuwyak.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/glnkkztdc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gawezxwsk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gfafyrtkh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gfmbwxary.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gprnlcryi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gfndnrvvc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gearujrqh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/ggbwuxcvv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbyupccav.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gixvqnemw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcevvngrj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/goqscmncd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gvmqfwbfv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gzzfadlxu.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gaejxiicp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gymupmzlr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gvocatawd.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gezmvplkc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gljirdzun.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gilrigips.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gxchmxjrl.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfcyzucnj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbctjlsdz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfhdmtpui.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gfflqeirs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gpxrzvbrs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/giowsbtqw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/ghtozvmvt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/guhtljiri.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gvkadmgdh.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gaqiepwif.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gkeuurwih.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gmbmcsvms.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/grzusfopq.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/ghimscaaf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/ghoyasqrw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gqyanmjbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gcifmomdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gzwjpkvtq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gkozqqdhh.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/glsidaukf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gervorkna.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gvajvotof.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gdjjudvsm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gdxoftcnp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gpyegyrfg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/ginngkftt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbazlzrpi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gtxvbngea.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gbrtryhin.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gkecmftaa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gzijpoxlt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gttfzcnky.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gfcxjnpfq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvvhjaqdq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/grzjgvyqo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gxazwwrad.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/glwuqvedh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gakipklmn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gyemobysv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/grudbhhfr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdqfhrvap.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gteyazzpr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gkncfqtqh.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqsgcsybc.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtzuzzltt.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gxlepbqig.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gbkbeqeyg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcqibczjq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gseinbnrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcrhymojh.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gusmnbmju.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggaydouxf.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gasnsltay.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gkchssawn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gcvxnisar.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/glrhemnfy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gluwsvyhg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gdjpagdla.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gcpnbmhzs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gynpsufvn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gxscouode.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gsafcllho.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/godeizpcu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/ghxzzqxbt.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gtfylqooh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gynktkfki.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gnkwccnjf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gkushqwaa.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggevywrlz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gvzubzmxn.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqwvsehyu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gewooxnvz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/giglulzex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfphdgvdn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjycmmmqj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gwxyvexqr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gsitgtyxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/ggjoznmkz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwahjuboo.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gofcujclh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gbmyticfc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gofumqpbt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqntrkwux.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gciryrued.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gwkkrtqhw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gbacgsros.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdfpyjxrv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghrntlaos.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gkkedvkuy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gwblycdio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gjicblfho.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gcyrlgwkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gruyhpzvi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gkndovfun.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/ggxuzzukw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/ghvyhceuj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkoqtqyxh.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/ghwtbcphj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gqiesgtqb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtjftqorg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gquzizzyq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmngnrqdk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/glztawdlh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxbvcgxnl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpwythmni.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdtfbsswb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gmfknwfqg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gafylaidh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gqdvyjjvw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gmykwmmjm.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/glmqyqxup.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gnpmuofsu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gvvknluyy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gwxxbfnld.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/grvocuzun.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gkncpeowb.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gjvmfwsti.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gdhnnfpvj.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gpsxbllnv.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/glaikqqji.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnlwezaqe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/ghujiawym.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gifhbusqx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghlqhuqyd.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/grcxaijbb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gddnjcbsb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfxlwexsc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/ghcxuxrlz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gnqzrgiri.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gmldyhzlb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gvbyglqur.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gpwfaxmel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfznirnzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gfwkthnju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gznbkyepi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gfypuanrk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmevscyne.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gtlqcrgia.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gegeqoucz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gskhivyfk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwzkucovi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gssaswezp.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gayqkpslz.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gvckmzaap.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gqdcavafl.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gyxgybtcg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gehdogskw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gqqidmfuf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gzpjhxpjj.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gjinvvyxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxbecbnxz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gfehxndba.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gryhkittd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gqszezohc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ggexdfrlf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gqznwlamk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gqmzufvrw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gdcknxrci.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gjzjdmatq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gswepjwfr.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gqrkjnhtr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gtlwewxeu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gvbdethmj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghbneygyc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkltxsuke.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gvcgkjyks.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gclatench.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gezfaphhp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gavtvdjnx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gwrwaatkk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gdjexajgp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpiamknsl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gcobxretc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/glzifochq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbioptvet.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/guwhmynaj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gxxteeter.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gpfizyylt.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gimgmspnw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gpzpxrrlr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gttikjqxq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gjlfihvmb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gplamvhod.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gsfvjllvr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gugcmolib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gjeivltan.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gricsycig.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gzkzxluzl.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gfgoywkfs.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gxdlyhemu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/glshufrjq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gublnyxiw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gvptvfsyw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gbvcpfwer.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/ggsablmss.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gfjxoqemc.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gtmtvnmag.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gcjiwxpbr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gcxuzpjzo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gvzcidhuy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/ggokkdbme.sHtML


<!-- 参考信息 -->