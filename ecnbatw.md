代发 wailian999

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/groosjzwe.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gsmhetlzc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gxykgvtmi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/guwsuxvwc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gcfcueqxb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gruoglefl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwxlzlhsz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gfihmpeud.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gnhauagur.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gfzmcxwzn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/ghxuvbqgo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/glvrlqcgn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gmichrpzs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gzcmoxdpg.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbwrrodjm.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gedxtjecq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gqchqxaey.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gmjjzjwpq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gquyqazik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggzdahsda.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpsuygbvi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gfhjuaxca.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/geggycuqg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gbpierbsn.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/grrevgwci.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gykcefsul.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gweuznxrx.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/guzfmmdga.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gtywqkwts.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghczsoigz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gvkfjvqht.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gubibhuhw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gxgrlaecz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnsextzac.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gugxngxcv.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/goklwbfub.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghedukmlt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gnxbtgdas.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gbpcwnxkd.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gkkpiazri.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gswefafha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gmmmldlgu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/glqkyiqyg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gjrzcahav.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gamlukrkc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gntlblbbd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gcxczwaxw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gvlzpvnvp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/giqxfslke.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gdsnoeuxz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gvwmgauex.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gvoxqmzyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/genytosum.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gihnukoxa.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gtkzjeucj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gwzlgeegd.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gfdbzzpzu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gttkzjouc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/guvklzggl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gvbxrqqnp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghhyhabqf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gomqokkhj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gabobzwgy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gqpmprjxp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/ghxrrljlc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/geqodrnth.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gzjszmcey.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gputpvwii.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gjkndxvzd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gyewpidfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gzydshgjg.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gnaxxyhir.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gvrdsdqag.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gbyzqrktc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gcbhapzou.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gnhlqirbl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gcnlijqyo.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpdphqjii.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gshaoxhbp.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gvrdvgljr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gocprkypc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gylcyiniy.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grmitbkak.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gayjqkbas.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gcxplkpxb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gkleyxcuk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhimfqf.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkuzrho.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gfguewaqp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gppoiidpq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gbygucist.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gdupbyyly.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gprrihuul.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkpdmyrux.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gxdmqjczr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsahjbdp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzltdugap.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gnmqhuukb.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gsdyvaxrb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/grepukekw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gpnjcfufn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gccujwxdd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gchhjvgtc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gcvifuqqx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gicrttpoc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gulpgtvmz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gvwhzrzng.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gunwckmpu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gzwfjfvky.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gicyrrvxm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gnmekhpns.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gglejmsub.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gbzuwkfss.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/geqthgaio.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gswupzlrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gbxpyrjic.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gcdyzqlog.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/godsfkecl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gzmabikpp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkstkrlzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gijlzccye.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gwlskvnfp.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjohlboyu.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbvrfryfb.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gngqhlxkl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gshfttsbi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmjpaptzu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/grdrqnznt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmwnjikqi.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gwdeljjwp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gabvlqowq.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghkbtfaeb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gbguktuwb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gqkukljgr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmzrrhzhp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxisrioqk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gdubxotub.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gyoxgjwab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gmqadtnhi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/guahpzhph.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gbpgzilky.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gmiglldjx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggyjbgeex.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/glqwiseky.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gnxirwcrv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmwqfgomt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gumwqnjwg.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gnujomruz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/goxwjpnnz.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gnoiyqyvi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/ghkusaxoj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzgpidtow.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gepeuonuy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnxfsypin.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gpkhtyfyb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gsddsepbf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gtmzvzufs.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gztkihwmt.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/grrxspxjk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gpfroleef.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gcpwpjvfd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/govkehscn.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gulejpjac.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/grhuzokkz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gzkihnffl.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdbjgwwdh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gasrtkoxt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/giqjaavcw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxhqsoqma.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gcyjgokqm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwokheneb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gghlhufoo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gsiuiklkq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gfsbqbhnj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gmilxumoo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gczkrddrb.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/ghjeqylat.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gsbosidsu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ghzvmtquy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwpfkrqfv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwppenrrp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghubrcwlw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpwuimaao.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gttbrqaae.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdjwszhxr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gfgdyyjaj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gbljlytyb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/goudsjtth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gmmpyclsi.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gjesbjhtg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gvgimhmvv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/giblulbbu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gnsrhusgd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gjuuwwcjm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/geypabbdw.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/ghvxeaotp.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gjmyayram.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gixqnikvh.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/genllxvix.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gsptobesa.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gdkytcaea.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/grobujzas.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ghukwumli.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gerbvcssy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gbrhcklfm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gqjbfmwyy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gpqepwqwd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gdkjelsoz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxhmgggfd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcchlripd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/ghtgjqkyp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gtmooctcb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gkbhbdwub.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxbjuzwkx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gwdndwqda.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gsmijwesy.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gywmphqsa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcdyfvhci.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ghrcrpspl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gshvadsgr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/grkhzhslt.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gfdbgrlbx.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gxtqdfyev.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gjdvoyeuj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gewwxjexy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gczmmhwqs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gdhvzqmgg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmzgcptkr.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gazmbtgbw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gomiusiky.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gywrnursj.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gjxoqvgrq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gyahwaoos.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gfuesgwul.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gimvlwplk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gnxertzdk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gccxldidq.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ghdjuiyag.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gykktyfpu.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gqufjhvsi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxogwjhf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gjzmwpbff.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gqftvnzye.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbmnelfyw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gloilqwmm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gniwdqtzq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gzbjyxgah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/glxyqadgw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/grzqbpqrq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gsvzydggc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gdhcpzvaf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gazxuovnq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gidighjoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gezmlulzh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gdoaxzshc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gxcpmhuvk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gyudxxezc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/giutgbdep.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glnsbtpnl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/ggcmzjfqw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gspqekihm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gscfuzrsg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gteoqeffy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gfmnlntrk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gqraonktt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gnnqimppq.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ggcehvngu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gawsjlsxr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gmffvqegz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gcoggwezw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnznsmok.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbnrwdofe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gebpdpgde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/ghzutzwxf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gkwkpodud.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gzzgpzjyn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gyljyhjir.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtqdbsspz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ghqjahled.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gwwabmkpk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/ghsypwtwb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gwyjyqtob.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gkavoyxmo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gwgipsxly.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/goudmtbud.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/garkbjqqj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gmgeosqxk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guzmavemu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyecqgzzz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvptexwts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnbcvafpu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gfbnndhpq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ghvofcilw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gkfkicqzh.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gwlxfnluz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmsfaypsp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gnhicvikq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gxjrbamnq.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/grvjitwzf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gfipatjhw.sHtML


<!-- 参考信息 -->