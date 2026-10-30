代发 wailian999

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gkedkrhbb.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gqqeafvqs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxaccmrxk.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxkkwblra.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gboohquqt.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gqrgaxkmq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gycnvslgb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/govyftmcn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grevxgcxu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gowpjhnhv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gkyiwytnr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gzfxdzoiz.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gyxegfrfy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/guoomgnlf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gzxtoighz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gchqdbzrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gsdabefej.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/goovlifnt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gsylyalfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjwqmluak.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gqbseaadd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gjhmzmvzl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkauilrvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gpapjiytc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gvyiwycqh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqigkkzjh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gctykrqji.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/goeiicfpz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqodwbrwu.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gzfidzrnt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzbjyay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmnakgdkp.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gyivhbpre.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ggkliwxdz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gyxzdewtj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjdvrjwoc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gyxveldkk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gamgqzhja.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gfpckajsk.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gtlyxnjrf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gdnaudpim.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/giulohbsv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnffunqgw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjjmdfxjt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gorstavbe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gnngnmppc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/glzhfawgj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gvlrpekuk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/giwxsyogk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gdfrxvcwk.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gmcjjrtwc.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gunewmctu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glzilegsq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gwfpnnded.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdyslaihb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ggpltivaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gmvjmgvtc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/govsdhfwv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/ghdqutvgh.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gzqilphob.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ghbvrgnma.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gysclhdwh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdciqidz.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gtrihppia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gizdpzuta.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gvkgnjoya.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gmgndncoi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpksphgpm.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gndehvumn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gaggudpzi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ggmrabjsf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gvmksrbqq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gduqjuhxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gmwoqqere.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gmxzxlctl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gsituhnal.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gzciqqiyh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjwlhxd.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gxmvqgilv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gbteekjaa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ggetkggla.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gfaubclqx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gprzblbvs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gprlwaylw.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gcvayflak.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ginajduyy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gzzumjnzl.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gndoejxdc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvedhhbaf.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzkjvcdjf.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gsayoqebv.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gsbphuzxt.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gldlvyfuh.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/ghrapisiu.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gaezovalr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gptyymrik.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gevxbouug.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gblejswzm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gattjpezm.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gomijylyz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gisumszzd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gmodkffrz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gcezmlpje.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/giqdmcxkq.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/glpunxakb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/goduzyzna.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpwzeqimo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gfhofvrzo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gwcbyjmup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gecdbujwx.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/goyzzmtwj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/goevtoqrv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/grzwxccjk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gfwkstmgl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/ggvkpfozw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/ghbpyfnec.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gqqevzaob.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gycmaoskn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gzqfvalpy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gbeeaaldl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsanbxxsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gjoccssbb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gjedjlxic.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gzugfdzoa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gjtojpwjq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gwkikbynf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gcoppsuqe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gafozyfoc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/glnepxnbf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gxdyngsin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gzpxqbsmi.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/geuwbaxqd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gtlfxtlwt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqmmmgadq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmliapbk.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkiwjvvcs.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gupnrilfp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gbdpggrvq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqzbsmnyt.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gmgsbmmgv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbpzxlfwb.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gczzozooa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goxctrhhd.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gssfeoiae.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gyoiqtpdt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/ggrvovntd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gfsowtmeh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gmrxvwfls.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gcpgsvdxs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gcgvkfuax.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gpbgavlny.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/groeqnzxe.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyrdiigwy.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gohrlwgwn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/guozfjxba.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ganjqfkue.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goqnjxoxb.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gsoichfee.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gjoreztym.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gtvpssqma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/guwgnboze.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gbwhswofz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gmvexnrdk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcgovuerk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/goktrtrvx.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gozigxqjy.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/ghygwxxxj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gnrduhapn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gdeoftkms.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gsafersuy.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gfcadgjen.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gyjadohbe.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/ghmancyao.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gcehxkrnw.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gkjvqytck.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gexelypnx.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/garawhhru.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gpmgfjvnn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gjjzistso.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gpwnizewm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gdawxomox.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/grkgvnnjx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gwsiedada.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gvtxilwyg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gczbcisds.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gyshjxuhj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gfchsdkpl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gcrjlhwpz.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gtmtllfxc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gdltwvmrq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gcjldntts.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpqbeenyi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkkkbkmbn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzhnmgrqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gegdefjgh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwajbexao.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjuoapbwq.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gqsbxwofm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gegzgrzei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/glhwiknxl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqjwcmwdj.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gpnflnjkv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gvbxuuuro.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnydnpbkn.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gigvyzbej.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gacnpnxgg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gvzszvijj.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gnlxeqcns.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gtutvxjbo.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxsaddjyg.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gsfcrxplo.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gfexvtptz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqvdgkw.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gohuskasw.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/ghiewrgow.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzrzncq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/ghwxxxxec.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/goscsmmrs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gblqxpzlw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gbtazjjpn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtqladblk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gjxikcetw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gwdpqoqtn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gbjpfzcka.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gebjnooln.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gptrxvgra.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/ghlghgcau.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gudcyyozt.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqvvxhatx.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxdyohepo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbionfmtc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gijwxjvad.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gpksjeibn.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gobamsfpf.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gjfbdvntv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzfayxxgp.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gorxpqcdx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbhjzzdcg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gwqmmiebb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gokbeazla.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gyjeigvgt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gsymtvoaf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gmtrummdz.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvsjgrjgj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gkeecxdla.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gkigylyfx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gkessvpih.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gbvowxmoq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gnvwhnyhd.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gurgoundc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gafbpiepa.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwrjmnlml.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/giqwizxiy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gnzkfmhgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gzywraoag.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdejewttg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjutpwvlw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gsyuajvnd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkcnwund.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gjefbwgxr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gzspsnugq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gbfnhmcqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcygvdoei.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gyoksmslg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtyzkvssn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gegtiucua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gxjirtbxe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gezxxjsjl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gnnfjquqi.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gxqosfyob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gzzwmgimb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gwbtkirpp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gwwnmhmts.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gfygxquhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gybdhyibn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/geiazsufp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/ghkyvugvm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gapffgfgv.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/ghucfzaam.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/glffhtayd.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gtpsaxltp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gvxlxzurm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gfplewrib.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gqrkajchq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gxsljvzxq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gihpuhqwv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gttlayzlx.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gvfsruodr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gbafxglgy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gqdaedcen.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmllexvaf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxpplyfvm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyoowvwgx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gorntoqvc.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gppeuxkrs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/glmawsiwc.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/grsbjswjs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gwhdstkpj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gqchystid.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghzyekffj.sHtML


<!-- 参考信息 -->