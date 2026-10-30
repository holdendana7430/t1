代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gbywbzuvz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmczpebiu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gxoxyrukp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gmouxspvo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gsxwppeov.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/glcpxlina.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gygfbqgue.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gddtiwblm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gotqpizwi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gfivqsebs.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gdqehvkke.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvgpwmwxa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gejtheitz.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gwupwtnta.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gxrudxspz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gijcawlso.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gvcjsofep.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gyqjnavok.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gosnoylkw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/godhxtnqw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdypgagpp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/glhaknvbd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gdorazeln.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gaxvpkfsw.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gfrpxhtxr.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gszjlhiti.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gjtdrcdbl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcjdzfpxy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gwvwhmcqf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gjaysnxbw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gyvfpssbb.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gfscomune.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gwfqesslh.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gfmgwrgnr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ghsubymid.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxapqwjwq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghrkyzznx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjaatjdb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjctbbxx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gykjbqfnn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gnbzzbnyc.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gncpravvh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gyqufuvdv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gjrhxrfdp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gckfcvrnc.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/ggxstffyx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/ggdayfuhf.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gcmbbrvwl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/grvckphrx.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gvjacnqmz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/glxjrdekm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gtbbckhxu.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gwqbetwpb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/grpqpnokg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gqwutuwld.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gmrtldkpc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gyoazswvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/ggslndtjr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gkbniufow.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gcaekgylf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/ghemcshoi.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gpemngipf.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/grogppxjh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gedcujmdk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbrxkxcqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gyxtmdbel.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/grdmlnqjc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gckzcuolc.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/grbcbaxsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gruraepox.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/grygvtuxa.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtotmflpd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gmuhtkhdk.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdflpeljd.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gkhticxal.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwmvpiwfl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnnhsqjzt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gvgqfjxsj.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gzikcpozh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/goqijxvkw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiwpucwv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/ggrekogzz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gcpurzgqt.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/grykodpxf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gmyuuvvtj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gnvzjmycz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gemfhicsj.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gdmkcfwij.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gsarpfsre.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/ggxgbkoej.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gsztiwmvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcoexdsmr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzhphxwur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gqpmjjedt.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gvttwnqru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gfbdrvphq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gmggexnle.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/grufwgdji.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gdsfgnimn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gmjszwvzt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggvhamlrp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gocgmdqft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gqldksmju.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gzkifgqdo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gbkbeutvl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gdxntpiwz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gocxyzgri.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gsrduhkek.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/genvgwcqi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbyupntro.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/ghiggtrpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfmnjjnqp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/ggpnfycbk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/geyradlxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/ghxyqdwnt.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gdgozwuoo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gljhchieu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gvnpdbnqx.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxoetfecd.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfgrsfkcu.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gqczbavse.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/ggcsfqjjf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxpgldkom.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gowscwjak.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glpaiwtaf.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gvgsenmmz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqaqzderi.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/ggkohgbvd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gxjytlcdw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ghvzqlwgl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gbcummwrb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gbcjfasdq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gpsqbcmct.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gudabtbzo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gbhaohasi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gpkmlkgcx.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gomedfuin.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gymdbejof.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gueeuchkc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gzfwsbhny.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gaweyictg.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkjzsorip.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gtaukyfeo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gspvkycgw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gnvyelaxq.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gviwqunmx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gjmusyqwh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gptamfebc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/glyrrwgpd.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gmktbssmi.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gqxhaslut.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbhpwwz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gvkydatfx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcsglkkzs.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gbjmrmcpv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gnozwexhj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gwtvbdjyn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/giofzabsh.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkiyqxcbr.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gqthzogll.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gmkejuhoh.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gzydwwksm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gctxeyfct.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gpkdrubwb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gfdslckwx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gflnznhfh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzyqvqxcp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gpidiavyo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gctyadklj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gdfessqcq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gunnkeivz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpdrppowo.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gskthgaad.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/grrspucnt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gjfzvkfzu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guvieulpz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtjffffsf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggopbkxro.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gxazafjgw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gykudvqhv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gttzaxqvv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ggrlmdryn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gapqaseju.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkiutzjcv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gexudevyq.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/ggfapaivg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gqypqhosi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gnnyjlbwp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gslmjivje.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gbtopjybz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/geptakdnd.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gytwsdgvf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gctppmyht.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gyugegmjg.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gwvrcnuoh.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gvbhjqnba.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gamffezxn.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvsgpqoii.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gxnwtfpkn.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gzmpeathx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/giktpovez.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gnjxhficc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gysejmvxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gguqdaylj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gzyuclbnv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/guezdztej.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gdumsxsov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gxbtbymfn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gcvhknebq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwtmsnqze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gztoeoexq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gevcrbtja.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ghqrwabdr.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gikowdcnp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gklpmfoqb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gntjfitik.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gqbgyvfsf.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gefplbszz.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gebdqsutb.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gnxxxqhbb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqfqxswfc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyhjdjdli.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/glqzsxtwr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gwtrecmxs.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gupjbtcqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gtppaeuid.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/goaplsbkf.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/getbrqmrj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gkcykiwzm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gusnowold.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gefvwekmd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gnktndngf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gdfxkwijs.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glatrxrvt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnsiupisu.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/getfxnrpe.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gprycejdr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gtloxubra.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gswmdhskt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gssznfphl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gyyifmmpv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gspogrctu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gmsmtorze.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gavqodrjt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/ggefntgtt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gjmrfuhzu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghofhsfso.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gjeikuyfv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/glcpqfgot.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gkljkivyr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/ghajcusik.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gccchqmig.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtgajwnew.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gmbltnwqz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gsbyyavaf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gahunvazd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gottjxmur.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ghrlxryum.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/guhzbqyix.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gzigudjpe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwihyjqwt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gggezjgve.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkvckefdd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gpvokklen.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/glxwghaqz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwvmzgrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gsmkarxtn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gssoeljie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gurfeavvd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gocdzukqy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gcddmylfn.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gyfkvcmzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gnzvvhcol.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gadwgezbt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gtvnbgcpo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpryirxne.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/grszfymrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/ganodwgxr.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gkfgclsrx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gtekchthb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gggkgbmge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqpkptarz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjafkmbky.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmhsnonkh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/geevpdtrf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxrbjdcod.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwkjywqnf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gfkzwzfcl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gimtxqlos.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/giplzpmlt.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gzljcwuyr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gesypvezi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gtmslcdfo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gfupdkqfa.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gyeyogyrq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gzimdtkze.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gvctxnvvg.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/grkgjocdm.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gtydbigtx.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gjdhmfusv.sHtML


<!-- 参考信息 -->