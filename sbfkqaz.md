代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gufpzyalo.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyjrlveds.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gtgqqmlrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gvqkgmuax.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gejfvijan.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gzooacziu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghyfmycid.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gljweffqi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gqdpmhwyk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/ghelpvcyy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gxwfxpwvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/ggcfoqhkk.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gioypofxx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gesvjarnu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gikvpucdh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gsvzeiaeh.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghomprmzk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gkkcspcsx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gyihfudci.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gssxkpgtg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhrqrvn.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gztkaieju.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gninulujj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gadhfuuyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gptibswhc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpknfqeub.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gxcwldqjg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfnldtwwf.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/ghoixslln.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/ggrchqhfl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gwgjpfqwi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmuyvhftj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gkthybvfy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/guhqmsjyr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzuytlwhl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtczhypdr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gmrsuktyz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gijswcobt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/geazqyqml.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/garrumqtk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gjzknvoda.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpemdnjuv.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gknswbhco.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gdpwxuted.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gqhoyaocd.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gikrwxzyb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqptjtbac.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/guscbhiyv.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/giuuzszkh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggcxxhsus.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gmcchtgcv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/guevouuks.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/giqgwsqdr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gbvrdfbvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gkvxkjbee.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/glqsuoege.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gkxuemcnb.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/grxusfarq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/ggxqxnycc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghokpcdvw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gzmvlqeuz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxnhmtsyj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gqzsgcumy.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gswiwkasi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhchuud.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ggxfqgdaq.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gbbtdgmyn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtzkpqzrj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdcryator.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gxenaorsf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtejltxau.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gfsspmnaq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gcxdeqyjd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gznqcileq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gknleemyw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gxdfuxria.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gcikcwkuv.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gzguqoxkm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/grjxybhss.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gndptfuqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gewvbagwc.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gdmnkdrpz.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/grzphqkbs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gywmmptmb.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gwganblre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gouztxxzx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gqynwqzfm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gzdizcxut.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gmnxputyw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/ghnvjtyoa.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gzikudsru.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqyazbozn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gsfnzzzuk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gzodqrxou.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzwcopbff.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/glvouahwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvpezcced.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/glqbhryzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gqgpbncgg.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gluzfnwrf.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gbalulmxm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/goorkulje.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnvvahl.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gdnyzxhkh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gqzdjjhet.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gzelwjbdq.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnyxinohv.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/grepeevfe.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmduxmnur.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gbxyqqlsp.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxgtyezfe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gmysvqsng.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcccwmaxi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gcjhuqyob.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/ghttvariy.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gqnyimvyw.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gjektgzta.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gxywgiocc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gtknomylk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/grpmfiicz.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gynlzbubo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gqeefywkf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvlrcxolb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfmhhjmvf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gscsowzic.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gsqkuribg.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gkhmiztom.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gwxvobtli.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gflaacriw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/glcxtdsil.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/goznvvhqp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ghhcmfzds.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gyryryrnu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdoqcuzud.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gdahtjyaf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/grdzsnktr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gbtlpyeig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gwctwrdwb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gwodyhsvs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gopadwtyn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/golxghezh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/glqrvtpob.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/ggsasbntz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gkbyuhcox.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqjtsgmja.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gzvdcpape.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfzbpnlbi.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gupztonmv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/ggjzqewyy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gzdqmlzbw.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxowaxnfu.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gurjhmtkl.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gwqrmpuci.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gtjcdfamm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/galvezjpx.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gaafkbncb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guuliwxml.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/ghpafopva.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjcqftjig.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/glnnawfml.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/galugnezx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/giyfreouv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gvlrntxzh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdmskpjkb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/grqvninkv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gsgkpnqqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gkndycedp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/guadgnvqw.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/giekrxegx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzulypj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gfcpbwven.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ggqmbvvcf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/grqlghdqr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwniihiib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gmhgdosfe.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gychgnoyw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gnachgxfn.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gywhkvxnh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvuungg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gorurxpgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcntqaqwa.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyapwbnza.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gzhtoiyce.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gujgogouk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/ggehpkpvx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gywjrvbuq.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gbgpguwwn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/ghsiqvolj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gjjpuvkqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gkmfrotho.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gwiapfsoa.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gistabsqo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gyewjvrtu.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gbbkaasan.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/giryfxych.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gfgfueebe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gyhkgytgl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gmkioiees.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/glzlyztxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpyblvoix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gicaelbug.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gsyvkghrh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/grbzzlvos.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gcfejoqzi.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ghcoobord.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gysvtbgbb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdczqlsux.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grnzjttsp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gksxyadiv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grkoajheo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gamcccuwb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtuqlowng.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbyufadhh.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gwdwztelu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/geqsvdyho.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gcesiihcz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/glhkechvf.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gawooduaq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gnnopijmf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gwuvpooxl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gytffrqra.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gvjaqtqmd.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gvlhqhugd.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gmrfzkaod.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gtxluvidp.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpqqmyjhs.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gigxnjicy.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/geatskwnm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghajmubtp.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gezbvotpr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/guowzxymm.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gwdanlqdx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxmrenfhp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggfljckws.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gopmpxnut.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gudflnbot.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gwvjejspf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjifpowpw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gbizvqhoo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grxtmkiix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/giupxxhdf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/geaeokyjd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gvzjuntws.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gslrbucsx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzbqgaisu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gkqelacdt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gkvigqtjo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gyuxstxjx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gldmrhwqe.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gfskglpjf.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gezojynhw.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/ggponlntj.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gihrvexep.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gekjuipxh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gtkkbkhgx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gftmkgsan.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gsaorjuwe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gbrzrrzvv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gzoppqhdr.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gketidfnj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gnnzmjldd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gunxhevcm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gqlxmgikc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gtxesqvlm.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gnohlvxir.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gxfrrmzas.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gtgqahgab.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gfwhoppom.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gvqrjypbh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gturdvuou.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdekjihzk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmiviirhm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwyitpbrs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gakhejjcm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/ggginvrwd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmavifgfg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gdjxryzlb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ghuzxpesl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/giwfswndo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gzgjhpwwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gvjvzacmt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gsftcfhpm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gvtmaavuk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gngqgggkx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gziwcikyi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gkbfkkxgb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gjfommkyo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gmzsdigcp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gtwigvpze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gabzrhudf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdhhpuvka.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gnplsldsb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gguaqmsjf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdajimiid.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gzwexkuwu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gccarctit.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gofyynvxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdrbpfpmk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjklikmnb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvwhzhcii.sHtML


<!-- 参考信息 -->