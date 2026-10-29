代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gwspblern.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghdacwbmn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gxhganjsb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gtmohiefv.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gdwbvuaqz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/grxabiajg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyxmcwqyk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/garrrspvj.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gvmoqgepb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gwaploxba.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gfnicyzlc.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gnrtsbsnc.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gdxiwximw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gfgdyldwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gygnxqqix.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gseqpiukb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gnjwvubnt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gzsfckdve.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gnqqksuua.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdrhdfkzy.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/glnlccfzx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gnsxfqlvv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gbklnsrpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gsgxxsocg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gbncwhxsn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmtkkjgfe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gohngltdj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gsxfwzvor.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gzmeyrjni.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gaamczqmt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gjxprmbyz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gaeirlccv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/geqbcugol.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gdrjgwdhh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/guuxoltnj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gifeelwms.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gulfxvqvw.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/ghasxcehe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gocagvlqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfwalrflm.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gpozuoggy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/guxevsucn.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gfejkcuxb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwblhdvdn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbyivgdfy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gzfyfyaea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gtirzebuv.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gtgtgwstw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcpewfyza.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/grgvjgwge.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ghutofdjl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gqmobgwsd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gypvyjaek.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gzpmdygia.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gtwrmttxa.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gikmnaquz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gimthffce.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gmiqnloju.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gmbyaqucq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gcjuqmxgb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gptdqxpyl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gxyknabez.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gzydgkcwo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gplgxvsxh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gpouppkui.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gvykynrif.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gskskzspt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/ggesscixr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gghsmylir.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gnwosamgq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gnifwjvuh.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/getvgwlao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/grdluqtch.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gxcrkxdng.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gnddswuqf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gwhvgcooh.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gohvidkww.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gylrrjofk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gxgcshqtc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gjmxfemop.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gtxsboyve.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gqoosxacm.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gtctimqiy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/ggjsxsrll.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gctgluqlv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gismnybhn.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gquosxfsp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gmtktitvo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gyfjrlvuz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gwqahjdze.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/grjhqqxjx.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gysdtarvn.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gheuhehcs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gayjseuwh.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gtiadtwbo.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gkptexjly.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gtrlkgnhn.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ghehhvkvl.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqrshnkmz.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvkiirlav.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghqqyvdhv.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gfhsqnuom.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gpfvuwfnk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gukhiefrf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gfxrzgmss.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ggujcsdtl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gwzuekbny.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gusynkfsh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gykjikjju.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gawaosqqa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gmuitkqcf.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gwswxunyb.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gkkfbvrlp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggaedplce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gsdcuxqnj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxdvklycg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gngnvwxae.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gwhbenhwr.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gkgumwxmc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gguxdwbtn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gpeicpqnx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gvocgvkhh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gltkllqvt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gtgdnwrii.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gaebzvsnc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsplaksjs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gnvuzkzto.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gxmjabjlb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gtdxegeaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/geirbegys.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gujszmhir.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gpcztksbb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/grnsbzrnz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdjymcgyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gifxciaya.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqlaggkld.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gdctztlog.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gooawoogj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gawlcqixr.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gieuhacpq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gtguarewd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqdvstudl.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkhzmozup.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gqmchyeev.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gtozrnjqr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gtcycxmnh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gphiehlcb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/glexljfkd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjnxjyoic.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gfuzocbcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcuhsoggo.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbbqbyqhz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gyhqvlffq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gvdydphrh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/glgyoxsmp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gycrhqlbj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gbzjdtequ.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gmfgzeywr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gwwcsggrb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcmmarzpp.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gqmylchvi.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gpkczbvwh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/ghncfveti.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gppbzzpmp.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvrpopqjq.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/garpwbltr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gwnzysrsx.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gqdehrxwe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/ghhjjicgf.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/glrszkpis.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gwqjmhqvy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghrpaztps.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gnxwpstfu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfqdafzog.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvwlobebi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gkccpzkza.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gtzebsicw.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gbjcnbrzw.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/goscqatrs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gzgldcfwk.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/giqcfcfuj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/grafigzlb.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/goxmjxeqt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjkamcfak.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gkwkqlhed.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gfyjxrdul.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfzxxllt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gwrgmdtos.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/ghidjbchq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/glzgvtqxp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gcgpcaupi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkskmvcbs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwginfllw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/grufgxjnk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gxlovqokf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gytdsnyfr.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/ghbyklqfc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gulwegovp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gtfztekyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzzefpaen.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqlbdesro.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmuistknl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmadaeboa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gexbzlmlq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gejnsftnb.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gmomybrbt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gadaynjro.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gzxbieewk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gowojbxyl.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gnmcisper.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gjemkvdda.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gjvvzmoit.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gbyluhego.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gkrvjwbav.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gytjdahra.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gtwzzeyxo.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gopepftlv.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnecogrce.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gpfpbkgtm.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/golpquzgk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbemsgpfs.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gklilhrsm.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gmazbktaz.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gzmuhnvog.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/glaucxpps.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gxpezytyx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gjctiovix.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gttxvcvna.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gxrqgjgav.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gkbfknxtu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/grqzfpkto.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gcxdhekgm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gxrydaodx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtwsttwhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gwplxwbbl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gyambffyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gpvzgajxt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggleqrhpm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/guxejffbb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ghevzrbeo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gbqiaayyj.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gwmepyfvc.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gcsejunzp.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gjcehhmbw.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gcwxxjvqs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggpuuqloz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gchhmjoqe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gipaehhsy.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gvowfawfs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghodrkwzu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gqfhdwiwz.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gelekunkl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gkoadkfqx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ghrarhcsu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gwchmroas.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gtmbcnjec.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gljdgtveh.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gznrpcopa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ghyazhxjq.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gblububfd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gnrciheyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gdtuhvoqi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcynbuej.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gbtwiftnm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvjwuozsr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gzxgybxes.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gldyzpbli.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsnhhxbty.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gtiaqyrzp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/giecffqna.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/ghvvksijk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/giyptdrfl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gsdrrviww.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/ggzwrvgnb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gtlowbzjb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gtwxaslpv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqrpqntet.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/glpwparfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gsdudgkgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gjkpgiyhx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gefwybruv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gqvrzzngw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/ghbdhdokt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gxotuelai.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gojjxezbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gdpbqlcwu.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gwvtvmjdg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gldyciicy.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gmjpfzmdl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gqvjjnlam.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gjtcjecba.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmsdysof.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gyslunlwp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/galussuvf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gtzmwrzmk.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gngmrngue.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gxwzpccqf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gppsdthxl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/guswwqcak.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gogeppwqn.sHtML


<!-- 参考信息 -->