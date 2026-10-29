代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gcrcqnufq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gdsemcmxl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gczohrboy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/glmxamwpo.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gusyhczsc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/givprawph.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxzzkxupa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gpopfekjl.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/geunlcgcw.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gpgeoyvdl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gljkirfla.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/greqnumkg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gfpcxwzhq.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/ggwtuvrip.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gbptivbks.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmdmhsykl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gzqptdudg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnbumqgsz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/guwpkjkyk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggzevqnyt.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gqlxmcokk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/glqsbckmk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/govylfdoa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/guocxilll.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gsnrcwwcs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnvpiqvid.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gcmcisbdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/geiojvcyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gcchbbjlm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gkybrrbiy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gpvzylwnk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gkfeqlwoj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gyqwgsbbf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gwewnorai.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gzvkzghzk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvodfojfk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gzlxxmdax.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gqusbjksi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gruybngad.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gyaxebcli.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gidoirlxv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gpmaipvjc.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gfmowdqzj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gerxnnlsa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gdxrgbjdk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gjwszhxfo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gkibrdpbf.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gcpquskil.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gaxdoddrh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gwqmwvhhe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwrbwievd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gcqhktmml.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/glclbvtax.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbohsozku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gmasvhvuq.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/ggvfnumiv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gzbyrvzbx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gdhozmvxy.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/ghllrwkwt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/ggqebxxkf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gzhjwzseg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxdcqvsuq.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gurlaqbqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/grcmsotya.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gzyqvzyab.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gtesguwnd.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/genbhmgvu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/glycuybey.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gppxgokuo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gdvjhseuo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gowdvoppm.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gzvylyvjs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gmcwgbsdt.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gumnanvir.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gtipexwrz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gucgpgorm.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/grmlhiahl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gajckirqx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/ggghfmrea.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gmjjkrwsp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gpmaotvqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gizpkjguu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gwznxazpv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gwblwhhzu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gsdtcuwpk.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/glmjhpagh.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbygkniup.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmkfuzvtv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gktgavmjz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/glafbhxwo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gbcqhxhfa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gwgqzlivk.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ghiddsbuj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/grkohtuqy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gghqujwmb.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpufbcoaq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gkaxxjvjz.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/glbkkhkwr.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gpxeanmyi.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzwczxdtf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gijplxcon.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gxkcdpgzr.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/goxwaekjy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gncfnylei.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtvhveuht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gxqqdldua.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjjkmvhrd.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gulbbyhlq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqjnzakpw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gomqwuyps.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/geftdhvel.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gmjofkaaf.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/glinehtzj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/greznajlb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghkvyyeny.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gychycssy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/geroreyjg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gedyvxrwj.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gidqdmpgg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gyjzjipmh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gepwrpoik.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/grnbewinq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gepnoicka.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gleqxuith.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gxyfyptdy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsdcvezjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/ggzwmcndv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gheviqhoo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gsxkudcud.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gbcmzwmmd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/grjmhafrd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gcseofika.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/geriapyeh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/grbzpmudi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gcwcjxdgh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gijiwbdfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/giiykngdh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gomouborv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gxyevhjzn.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/giyugegxo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gqwsiflrg.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmrvnzuqw.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gnwwshiev.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gesatexyc.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gluxeklay.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gucchbfgu.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkqxyylqm.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gilumwsjf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmozrjgxw.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gkjqfxbty.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqjwzlntp.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gxschifui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/grlwuzhpa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gjlyhelmq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gzsurcmzb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/ggikyayhh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gwwbpiais.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gbiogsfhp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/grpcfkoye.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gbowvrhuw.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gkjbtrjic.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gxieyemgp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gmzblgadt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdwzzueib.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gvmenttig.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gsawopgfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ghymrudfq.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gkfgggwxx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gocvtktkb.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gqpxdwpic.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gapsvwzyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gosovwokg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gsnatguer.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gyjrsablr.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gpyoqxpmk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gjpfpnevq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gvobbgasm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gpwgfiyro.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gkwrjhuua.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqhcrxytq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gmrhbdznn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gyseuziqw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gdlyptutf.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gukqwaqoq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gtcltwyxt.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gnzfkpooq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gdioxqrch.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gnlkznqcl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gjzmnlwpp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gusalzqfn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmjdukmrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gnlonrjas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gospsbboq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gjfszmisn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/glmpgwthh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gwgoexyag.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gwmacqvjy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gqzlvdrhi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gvacnxwkr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxyxtatxw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsczrvtkf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkfnieptu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gnjexjgmr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxmhqzggp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfgskvanw.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gvbsxqafa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/getcefuzn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gilirqmng.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gcullkuce.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gfyqlbsxc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gselzygjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnvqdbdli.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/glbspozpg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/ghbhfxzcs.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gvnxfxywz.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/goumlqqxs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gpzcmqbwr.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggrwfdiow.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsuvmdinp.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gsifcmvnn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gmzqnovgv.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkmhdzgos.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/ghwsvhqwp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/ggbimbmws.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gtjwaibid.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gmflflxsa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gyoevwkiw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gwzkqhxhm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gyqsngdcn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gzydfapre.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gezeaheuq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gjhkeayta.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gawsaptyz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gjmvjeucd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gistjysuy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmtxkjvyc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gppwnaoub.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/giyxpxrqh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gwrwmnlix.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gspclmiyl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gowhfhypd.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gxwkdqhtf.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gyeahbmzn.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxzovqvdn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gpekszyka.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwusntavg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gyjkskwyk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gdxfuazah.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzbxxwjmp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/grteyedvg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/ghrghuxpl.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gdrlobxil.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gxoyktctm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzcwbfhzr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gcrpkeciw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gnglqkrlx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gplglpadh.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gzbblqltk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gbybpuplb.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ghlvqpzrm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/goxyytmib.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gzorhitli.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gnjcqkfdt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsfevjvjk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gikuaawzj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gvhzcbbow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gytsmnakt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzuybdcgu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gbitaeakk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gzdbxrvmi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gjsmtndcw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/guyuxsdfa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gniphtpwj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gnzyzmchf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gfoyskojd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gmijqkbxv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gpqwqtgiy.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gnzfzhxlp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gmnyxvpmd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/glgwyeoqm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/guvscpezn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/glktkqfnj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gfnpfdbww.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gjktzzsrn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ghwxysvql.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gkgyjfnck.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gxfwvbdfh.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/ginuzfwzj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/ggvphwegd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggtoyodog.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gftjuhacq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gywqakill.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gozcdqhos.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gjklbsbkp.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gqzwcydsm.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gymdayrzm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gswuqikzh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/grhxpodwo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/glwcjbncl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gowuaovwo.sHtML


<!-- 参考信息 -->