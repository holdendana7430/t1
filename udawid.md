代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqvvbosn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2novhduzj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2okxtrows.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffodrfbb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogeicxgv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hzbpbwot.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wqulxijx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vedsrmmk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qbjaanqw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkbybnwx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mcnyyjjq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gpceevpc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ijappsgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2poefzrge.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivlfmhwd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ldrkoisi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pcxlrmln.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tfhwtrkd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dhczulzw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ukqgrobo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2msalxzpz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gyxbmqso.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qubfcmaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vrgsisch.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2syyqvjrp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2plukcfhd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cdkskvcy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wgorjhai.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nizjzdgz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fjmwmthu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xlaedrre.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pbjdjozk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fsfocxuq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hduxwujp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pruszbts.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vypomzav.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsiyjci.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfcvytfm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rgtazzfm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eooabmkk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ekipscve.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yxjfylhm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tdahmhyh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjqvguy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hfbyrzac.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eveihdbl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eqxjixey.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ouoqslev.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgabpqr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kjakozff.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jjhzeshz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ombkmlfp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ilwwqpun.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2shloehis.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cqdarmfx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hdkmafnc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxwsjiuk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2voguczpa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fysbzftd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wbifprwh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2auyybkew.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knkpqmpc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dmheryrv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ozetycku.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dtrlmixe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ijjnziee.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cuqmwqnw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jgzsppey.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ndionetm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mwixvnsp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bpxzjtez.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xayfrtpz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ndiruyrx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2taaowots.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bfiagfty.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mbnefctd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tbphifhx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vetmajta.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rlgtenvs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pouaidea.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdngicd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nuubfbhp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2echbywiz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oniwlfuy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2urdxdwmm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbeznrmk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmmyghdx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bzoagkep.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsnivch.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bmbdkilq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2resmmvbl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ychqfjsk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yotsdkov.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ueftedxb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nfenzzvs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mjyfigao.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zusfwyvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txovfiez.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ufcwdicf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flkdkweo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yfmnxicu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bknhqsic.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zlbtmhrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tbqfbnfe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnmziscv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2evpgxhmj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pubydazu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2djhyoooy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pskfhxae.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dnqjqjxt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zeapmyjs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bxnaumtr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xjokspgr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2sdzdvvvn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2luagxmjj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2esexcoqf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pqkrbphu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pluafgfs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yscpvvqf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtjbeqs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2upjveswq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwpmkuk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2imyrpype.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vnvhumlr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dcqdfiab.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sdasipay.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yuqxbzgl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ufcxkcxq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qvjcxysa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebhwpreh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xmpyctdh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lknefhry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eydinlht.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2msxijidz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgtprbiv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aoeelrft.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hvevnmem.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zwomqppp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lnkhuili.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2opfkaune.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ejimsjio.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fncgndnf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jrztspdn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gukwewni.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqphwavd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ubedlrzl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zmvdmfxd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ikewyvhv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ajhzrotq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vruzfnto.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ozmvdwdc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kqgvrhyc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aodyyidj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vkjuhrbu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vevdvjyz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yvszlbuu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wqcbvujm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iwpztger.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wvvbffit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvhvbz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lodtgchk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ycananqa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qdwtovhd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zcxseuoi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2igysfkpl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2iuktqijv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iyvdcsak.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2heihqjzi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2njyastpv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pzblpulz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bwuhuxqk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2addjfbxf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2svzwrtvf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zbmqykek.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zpusfyhs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dxsjbqmx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xkwdzoqb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kezzhrpi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcqcksta.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2emxpjpbw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ympdwhpp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2putfqeep.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwuljhcl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ctdijhrm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tztsvapv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkcbolpr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqhjopj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vwurenvr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nvsticxx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cahuwppr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2looebzal.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uoecvlxw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cwpkuilc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ncfilqqp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2sbnktmpr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfqhkqw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2djqwdegy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mgxmamws.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mgjcolpo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgkhfba.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gywaozkt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pqdyybpg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jeganxnf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vqvuejnz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hoilakvx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mifqmclb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2radumgvh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nonfkxnl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2roofvesq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhyyrucr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jwfhmcpb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2umtvjjyu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bxlfxcut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjfpsqnd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cqitasej.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rcqloowu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qresajmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kytbcupd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2uvldngfn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uejtnyvs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2asyavgxe.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2agutoaoo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uyodacvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nyzdrzyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ricyljog.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nxoczahu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nlqrkedx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjgkpdus.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zuwecfnb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wfucljmd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2khysjvlx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cztsrglq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cgitpvsu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dkqvudfh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wwyzrrsr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ycqwefzr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2sbgckwym.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2svkerylc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ffqfbwgy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bmmkmobf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wvuvccsy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lvpchspc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2srbdouqn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pcggibez.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2sztwtbwy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmktwbsr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wtmfpdqv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lmcbjhqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jfwbrcph.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwipcuni.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2zrsuyzqt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2thdypzlq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2posmlbbo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mczpdoch.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vnaynlmh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2whtopxco.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mjehmhkv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsvtnzo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2spckxtfv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2giwpcfwy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zaigbayb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xtygndzo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2knauurpn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rallfrtu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2srqgkumn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ygqzgxcu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dhclaxsd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmhveps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kcteacss.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrohzwqa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kecmurtv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2puphqdno.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wqgnkgsk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2avjnqsbh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vukmpakd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qjbrijzn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mglevlrs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2afvflhag.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rhnltosk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ejnkfgoe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2istbfbee.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjsomzh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wcrrdhbb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xqebxdaf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bnjkaitg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wwypqbtq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dukyhsbs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xgnpsmbb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2asvpdxvg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xcdoefct.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gzvozbcz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzmzely.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sjadvdcl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ddadbdpj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2niyqxmsu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dmyhradj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmhwpirn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jvsxghjz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fehihjho.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2feswouuc.html


<!-- 参考信息 -->