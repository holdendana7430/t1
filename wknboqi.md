代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gyhaafpuj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gstpktcrz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gwyksemya.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/guqsldnum.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gtbryuafy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/geptxxswa.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gmigkpkol.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gbezokvei.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ggfbzcsef.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gnrappeuu.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gewwafzmr.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/grcmfruyi.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gaogcslax.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gyjnuaenj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsddfglcu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/geimthykq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gzqhxcjlb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gltityiav.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gussfiwfd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grjspkpeg.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gfzkguxbp.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gockgdepw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gdcjxzllk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gfxanahra.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gttwbkqgi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gucwftikq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfzjqdtyu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/grvknxfmt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gmyfshlra.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gusuaxlff.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/guffhflpa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gzonzoxye.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gjzkvxjdc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gyqsedytg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjfhkgruz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwhyokjur.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gdzaoumcj.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gwroqyull.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gllmzdzdg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnngwmnwn.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gvnfgaxlr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gunnlxxun.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjkkvjmjc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gwkadtrgv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gtughafyu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/guvhowqwv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/goychamcv.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gdzccgrha.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gerfsdjfb.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gczuffzkn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gyyvcchba.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gokcvwrag.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvurpvzcu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gcpypvsjy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gjcqyolgl.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gvjqyzemf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gygwoxdje.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gtfgreiac.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/glsrujaeq.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gtoyunevt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gbejoehaj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gcfoyutxa.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gfzintjta.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gqkpuzddc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gmabcplya.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gykxfvpnt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gdoeztfbu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gqrikueqo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/goqklzuns.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gifdjweoz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gmweiibdp.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/getumylqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gunctmsbw.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gtdtwkdqn.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gjlbqoour.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gzeakdpew.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gtjwvrxzn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gvtowwghm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gnanfdbaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gupvtzxsi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmyxtzhhi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/giwyrmpil.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gmcegjupd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gpndjoxnn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gzjdbidjl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gswhgljue.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gyouwzaqm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gmpnwtyhc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvzomnprg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkezmwyge.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gydcenuns.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gwfertirq.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gietrkvcl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/guywfcftm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/geikslccw.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gcskrasjs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/ggdcfadxi.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gceehnlig.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxxpiqwbb.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gxjviznwo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gawdjarjm.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gszroadcu.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gafrkqfll.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/grgduktol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggihwlwte.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/grnekxquh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gfvplhgke.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gexzmrtpp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gzxpbnedd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/giqpefipt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gcybgnhec.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/geeueihft.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gylpyyepi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/geohylcri.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gdkezqxet.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcezvucrt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbzvmuysl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gjubrlelc.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gnarstivp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gtmxuwzuo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gitpnvclx.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gpnvtmclj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/ghyxmzoyk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gndtavlll.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gdoeivzvx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpwvmytu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gcqvjgdxf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gghdhbwfl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gbmbgvqpd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gfsvprqfo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gqayvaoyc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/glqrmkhql.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gubjfeimu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gflwjbxvj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/guwcgsxbx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gnfcsioru.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gafjxhwmh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gertrhoil.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpnjxboix.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gugqvajlp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gadljrpun.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gjyrwsrud.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ggeoaudau.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gkrficaph.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/ghalxjfed.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gvxwdyhix.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtdexgzmd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gquatsryp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggjfreyqd.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gbwhqpypd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gajcafqoe.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gduihhesy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gdsnreobj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gpefrsnwp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghurhutuv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdwfyydiy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gjcelmrls.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gqiaxpoti.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gjatnopvf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyxzujzfz.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ghbbqvzlm.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/glqlzadef.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gyvsvmdmf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzzgkrjct.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxyjedffe.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gaihbjtgb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gusacgkoh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gifiddzjo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/geddjiaxc.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gujfitqxg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gtxsajgzm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gcdorrntq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkknixofe.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gwnqmssyg.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gnhoqnwmf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gqxvplror.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gkvcrzrsg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gwtivfaoz.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/guquilsjf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gmtmygejp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gdfvywgxn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gaszlfwgw.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gvgnfwyhd.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gzkwejtcv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gwbncaiuq.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gbwkixgbu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwhhmepvx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gbsiiipqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/ginfaqcym.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gublwbhdu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/guntnucwx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gpafzjqrx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/grbpdcdqy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gmjykeixt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gnexijqho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyxpcxqod.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gcflrtmmf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gfnhjuiqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/ginwhspec.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glufvrzef.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/goxkfqfov.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gydweuxom.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/ggjthddgq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gedmdbwep.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfkqxjxpt.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gxxzwlhvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ghlbnxpcb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpdirqkky.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gxavkqudu.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/goiqtzswx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gycwvjssr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gbgcvebhx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/glshuawpe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gqfjterwf.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gulcebfnr.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gnzhlbuhv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gqsowabkv.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gahhagiiy.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gyzmmfivy.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gyldmkjgm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gbbhffocn.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwcadhoet.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gpexrmcvx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gunicljgq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/glmdtizxo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gpstrwgsd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/guxuibaja.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ghpxnsfhl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gtqpvnfsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gqfixgovo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gfxmwqhrw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gphjmxdgk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gtmdjqmpa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnbtudpkc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gvckdfdqq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcqsdqhhi.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyrxtfual.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gyruqtnsv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdpkecedu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gfhhtkblf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/grgbllpjv.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/ghllawukn.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/glargglvg.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gxvymenve.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgntadwn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gwbljgnfw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gjikhseht.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gjebgcjnd.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gervtganm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/grlyreuxj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gxpbnfsar.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gntiiieqh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gljnbsxhy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gcwgvvrxh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gokqlvmnb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gmvcbiibp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gqursaxlt.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gilhhadra.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gzysybtmn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmredfvdg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gupatnglm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/glotoebzf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gnmryfeno.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjclkmmcl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gmjxodqfw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gkpisrblu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gjdurrurg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ghejupard.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwojisggj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gtspiprpu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/ggufosvrv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gmedcuoxm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gvpaiqtbt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdwrhswhp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gladftlil.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gzfaxmrcz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gxdcavdys.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gybwsxbhi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmfnfodlk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gceegithd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gxbifrtek.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqlralfeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/ggplcnnkt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gwmqplqku.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggvuctlgz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gdpsedhod.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gvdkbmmla.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gocqxnjmx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gfancczyz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gzzvmzujc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gobmwbfub.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gycgmxvws.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gddpffqvs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gocwudcwo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gpfwyedaj.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gjpfcekud.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/genzdwgys.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gkckjybjc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/grgnctibg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnzinbask.sHtML


<!-- 参考信息 -->