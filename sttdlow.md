代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gsjsggfio.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/geftfeqfm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/ggnjfrrda.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gmeklcdjm.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gijacsile.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gurkqgetw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gbvdebist.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/glnognxuf.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gimpcsocx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gqicomibd.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gyvgogwtn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gcnjnvtgw.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfvhmmmhk.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gwyvktozy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/grsozubhq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gaaqeqieq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gzjfsdvxu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/glerosdsy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gqsbhkhfx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfomrlkdv.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/grbxklqsi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gesdsjuod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gwgnvglnm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ggtxdarkb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gglzkzrhe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbnljmkmk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guwnpdkrw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfcthxokv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gncwxhpyq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gqymgclnf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdzvqtmzu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gnhcmdvfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/grucsmpoi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghcvwyzau.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gddyrplxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gmygdhlut.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gqhisoadt.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gtwslguma.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gqwbgwtxx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gewscztzd.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gphfaciol.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gxohchaqf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxqizwsch.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbzuudnyy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gblpgeeko.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gnpawppwl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gwhnldmqb.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gybiwakqb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gugiabzbq.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gmrhlzaaq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gtbyhpqyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gvqwkwvim.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/grrzbwexi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxflpynfa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gfiorxnys.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gmueulrvo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gffsuxexc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gtlzeibpm.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gcavvheon.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gwmgydyzk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grlrlziyv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gncieuguh.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gfdqedznf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/grncmphvk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gvlnigqyk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gqskkahge.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gcphbehge.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gqnwfaagx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gaarjzkyc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gpvtjazgt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/guobuopel.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ghlwrmulx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbljbpkhr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggqymmldk.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gskbjpkom.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtmijroxc.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gdoccjzsn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gpxbrhxpu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gjearqknn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gqnffuscv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gzwjdyzqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gvlbfkfbp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gundnahet.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gfzqbqwrm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gxnoajznl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gzrmhxvpl.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gzytqmlli.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gwvtkoxoy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gmtipelus.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ghcxdokfq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gaztwdscp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gyymriwis.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gmpbsrfku.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/ggttxqrxp.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gstngslbg.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/guttdbrbr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gwdeytetu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpeugeaqk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjdoihyj.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpfhspuht.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjtyuubra.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gjxtfhdqo.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmhvahmru.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/ganiottbd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gqtbziceg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gqfpxpkzh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gbydzskeh.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gbzfhawyb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gsufnrhrz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gckwscsfi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/ggkrfzbft.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gzvzputlu.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gbrqihwga.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjizorsxv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmewcexb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gopspzvek.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gqxdpzlhl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/glzmtkaau.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gguivcycq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/ghhqandmr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gdnmgtuiz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gvaeydjox.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gnymznxgt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gcvuuxdnz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/geittgriw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gvigynopx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gkdkuidzp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gnfayoffg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/giyuhcpyo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gohrbmoip.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/glypapsfc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/glajxwlar.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdruqygzb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gvajdrrgo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gwqvrdadh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/girtcndcz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gjwjwbvdw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gonopmzby.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gihoklsgw.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gsdnsdkrd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/grakfbvto.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gbpmnmauc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghxxojoew.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqyumjjog.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gkoxddczh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gidfhnjza.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmtbmjdjq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gnsvxucch.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzvvqlteu.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/geaxiwueq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gachoucth.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkaknjbga.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gcwpzwspn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gdfwikvpe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gifqcloku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/ghxhuvggt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gbxzselmp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gmnteiftw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gsbyeexvo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwkclzuzm.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gzrtpbrdd.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gnsrocssy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gnjdsgwni.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqjhegely.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gebxsqgdg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/glpkqzhuk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gyifujiyn.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/grqukrsny.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gqtlcyxqv.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gztyghghb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/glavsxdpq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gouuuddin.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjcbcfwbm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxhauejo.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ggibgtbyu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gsbuzkdzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gryiteebh.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gzvhjdydn.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gzxddjjzd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggbgmarst.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gwgblqexx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gxntjvxns.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gjajqdbzm.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gqhgttypo.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/ghnqjvxmr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmdpxggtt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdhcsnyty.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gnlovixyp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gbuwcrwcr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gcjfnfths.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gapjjvtpv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gkyfpmsoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gqbrijlgm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gqiigonou.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gefpxpyhk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtkkncnoq.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gdozvjxwj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/grbbpeimo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gcoxohekf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcmlfpetn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/galmdpiuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzgrsttor.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gyycutavp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gviljvipm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grrocmprl.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gnwzowxlv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gfbaoonly.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsfvnpgdm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gcmavupmp.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/ghpxwmgoc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/ggsthoeic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gghlrvkgc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gyexecioe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gfkpgnzgp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gqhlewylx.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gjmgspkeq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gmwckderq.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjscatllk.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkxdveuoa.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/ghvgnpcev.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gbtohifcq.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gxyegnlgo.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gxmicaupt.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gxkpwygdm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/godhtxaoi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjzowpiux.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsamrsrcl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gojngvqij.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gqtspxiko.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/giogwuijy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gznhtytan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfoyajxky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gbrzfnrmq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gbhidzhld.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gaufdbrce.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gagobcbcn.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdnmpeeml.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gopgbhuww.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gymnezusa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gianxendt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gcjmbojxx.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gvnmgelue.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gqznfahjn.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gnsmupalc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjrlmzesb.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtesdutbg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/ghklhlqfw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gbblarecq.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/giclamnkm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gzxyxcdvs.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gwcvyppbq.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gxgtyhnov.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gaexkaufe.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gbtkxmpjq.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gpuyypuax.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gilnvsmgv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gjfezwbzn.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gkkneejda.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gvswgatdx.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/ggacqmauc.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gjaxbobjy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/ggbyxuquw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gucxsmcep.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gsklplqeb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gpzgxhezh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gyqsjxisv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gnbgznczv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/galczasjl.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gdcbhtlzp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/grkbgjawg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gssqkmvoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gqhpeaxdd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gaxrhgiyo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gcwyhyikd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gqnpgiyql.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/glgbscjqx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxbfhiqyt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gxlesigwq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghmvmjfjf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gpeenvtqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gepagtyih.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gqkfgeaip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gfvqbhszw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gmzgchzvw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gtufijabv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpngiagb.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gmrptzwwu.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gsjacszem.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gvwpcrxsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gfkwclwhn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gsbduuohj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gxjjjwhwq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gdkgecihs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gpzomiqvq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/guivibaeg.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gvrfpinqo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/guockpbxn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gqgrsqehh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gcmjzgvcw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gjrfmzfen.sHtML


<!-- 参考信息 -->