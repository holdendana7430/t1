代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uabnkchg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fxvqfdtz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xbrjusns.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jpwqhzkz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yfgnkjiu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rkrefzdr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgfgjoqe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xreqvvve.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ehmbwtbz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rsujyyej.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkubinl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plhrlknt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpoyefev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ylxsgkjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2etapphkd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oylflcca.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dlmqkjev.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gjvlnyml.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2joidrowb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xzjhlobw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tkvmrifb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rqgxfkkm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2aakdyrys.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tiufvhzh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pamztnob.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dmrpziyz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwtvkrxf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2balvgmnr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2crexzwfl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoconci.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ozyjedeq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hywrhica.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hhyxmmfw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2frgoaplb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2heffyufd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpraidfx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2afpzidqt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lavipnkn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ziucfegu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbxdcgys.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rgnhjmnm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vqcidvui.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rlgwkjav.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2olprfszg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cpshuujb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bekveecb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ujuyzjru.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zneibzpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctakoptm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zbeovdym.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fzvocqzn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmibaiwl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2igeepzai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dabxacfl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qffnbnbp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mamuojtn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vvgerztp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lttfqatv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kqywxtfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ftkbisem.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dlcbeznj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nrnkogyd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuoopai.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zoqdbcxl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jnfsghde.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kylontaa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xaaoskll.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ljmnlccy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2naqgersv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qlkzrcvh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hxrlrqka.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rysevwpz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfaiauw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2teuumiww.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lnjcnadc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ilchtkab.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cypwdfpl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syxvcjft.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgqncml.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2samaezcy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvrmmulp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vygfzmfa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gxmljwut.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rlmzukbv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lwgiinhx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nbrvmrxy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sjsqtdtk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2swzhhpmo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vnamkuyj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2cluaqivg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eyctusro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2thqyeskb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxkyvbi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfpcgsc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ofzogysu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dnajubye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2opxlthrp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vdaujadg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gfhxoasc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xsneuddj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2prcbrcaq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ndlhqdnn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xbkoqgdl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2idzdtimf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xcnnuekz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pewtbhsm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rugxfnjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2oyifrxvv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2havineto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bhwbrgdn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wnhdezsh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mfubzgfe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vedfycts.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hnxoglsa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nrqmmeuq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2syypkofl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dtsdloxp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ktebqywd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uedrczsn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fmytlaqh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2taseoivn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfjkbmkb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nebrdyie.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wtydfkaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcvekydn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2shwaadqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfxtnwiq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kmqvhslc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pvootara.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dtucfukk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2esdcizpt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2idcywnxn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cfjbtsxj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ykghqjky.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yuavirsq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hozsgoyd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zjusrkfd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2buhginet.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cepmempe.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vmmuajfo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uepbgscr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cstfnwzs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2arrsuqot.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2psdqjrtx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ojtkhdke.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2idtftxsd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wpcvdwur.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yrphtovz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qecenuzc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhjygogh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yrgrfpkc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kcravuzk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ubpxkoej.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rdibodvs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iwoirryi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rbkeksmq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bhjjzooi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqfyoim.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jseiporw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxorzvqt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gdpfpiva.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2onvtvams.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ckwhfmdg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fgldavvo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aecgimzo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2exrnwfrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ygbltprj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hegjbove.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ypoubhgv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2iorrkgph.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2emonkpwe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cixjtkyy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2megoljic.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwzfrhr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trhtgrem.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zvbaqqlo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otdbhsuf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2psoldizq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qerczokd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uvkhdxsd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxngfs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kwfbyium.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yfjlqgah.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xebxdsjt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2onszlsup.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bdvpvrxj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2damqzaea.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zgqtgykq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xdjotrqh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2aijasuzy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vdduobpp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zuibghdx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2swolpjvz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pclayimd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cxpodpmb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yckhdbig.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vndnrlco.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ombxirur.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ggytdfxo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wxltjunb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwwxciry.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahnpvvbp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2woshbjnl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fxzbjnap.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmqcregq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vetwmnrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2feazzbau.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2klfuiklo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rdazpocr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vkiybdwx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ioohvssn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2scyphlyr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qhchvutf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2elvniokt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2udhpdedc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpnunqu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bcteolcn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gzwngwkk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2swsinbbb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhyhlaba.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jyhdbyun.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dpusplsx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mbbevbkj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ylqssvlt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mbghdybu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jdudaapu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oitjblbi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bgojxtrl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gjefxyul.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oapeepcw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zuytrfdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qcybqanm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2njantrms.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ynifdsca.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rhugsetx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2imwlzfdr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2nbnhzknr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgdhran.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkkikat.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lotwvjqx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dizynzgh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xmsrpojy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xlralflz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zorgityd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ugjjhreb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fvyezpiu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vuxjpgmc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhyopre.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2osubfieh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2opqufzzw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kvgjsazh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mluhhncx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aeubgncw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rizlsmcw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aohjzvpy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjzwxdjb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wryyqpbe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ngwvropk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qovoyiph.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hfpuqfhx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jfzjkumc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zyldtuct.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2stmlhcyd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2girrcxqt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lqdmhkjb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2evafwbbu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mcerymjl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2askfooqn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2esrjpuia.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2iitjzxhf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lohfchnw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2snqdrxuv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2omucattw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2scrsnwnn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etbgdtlb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mukpacbu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omdphbvt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uadxxqtb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qtoevyci.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2sfzizbxo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vqtqzcan.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tqvutuvr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xaxkpalj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xowodtuy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlsdxhf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mwfxpbxu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhyiocn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2udpjywzl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ncadthhk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ggnxxkmm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zkxtrgjw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fghfqnqe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmacjbm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bsmfiztr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bjtuhdmv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iidzazcb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ifztnsmr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2foguojut.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2emxxtwep.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bfinjqae.html


<!-- 参考信息 -->