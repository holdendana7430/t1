代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jkfvufqe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fdzxkizu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwztrywt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jqyghgsj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3moqxvmsm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3izodeqwx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cwvsupmt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xteccyhy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jgzramka.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipohotjm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gtqozemn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3clvbpiqw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wehqzcma.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yztjxjwm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3itxzbazt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3plolqmob.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpivhati.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cmdiachd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3suxlamhu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mwraimqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3farpiemp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uprwffqq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkdmhqxp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wmoacqol.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxbbtngn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lsjxdcqo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yafzoywr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tnjlehpu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tsuanqki.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3umodoknu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qdmootlc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tkrnhkzd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ccclilhh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hnnsnjrg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkjlburs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zfkonlta.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xmuveero.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nxtmjwyz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bcgeoyie.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3memckekk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lfkuuqhu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ozeyofsv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3utjzwonf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3awioymak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpfxjzmr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jgkmbmmv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kksohvhm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tuwfwjyz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qxuzredm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3oasavrzu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3aqujefnl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtkcifok.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oylujkul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhvsbzy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inyhagsk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmfkyjb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrioijjj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3klijqxns.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ojrcrmxj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mexrshdp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tagibrpq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3omanpyxc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kfzdglxj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hgcobwqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jxtbgwuo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zddasjdo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ojzsdtft.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eljyhqyq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3akustwai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhijcwmi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3urwonofa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hnlkhiuh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kmmnzeiw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fqithxpc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hnfrtaxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pnzycxic.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iupeeegz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3umxqxnrt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tiijzizs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfpylooc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grfslmej.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zarnyiej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yhztgzud.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wjcmjkpi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3asllgrpe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ufuzinjz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mxxenvit.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3icqfqebj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3njtobczr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3llmsohhd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fobiudwi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eypyighy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlunezre.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwkhzvv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dptavxww.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3opmfifzw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeptgweh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uwxxnagv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfgemsve.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ykfskxmy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rrrvvydp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3stwcnpxd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tnwkkzgk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hjuvuvgm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mretnxfe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sitpikgm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3lluxbyst.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezmdljaf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzwblti.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ogihvmiy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jdeacvlc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3futmcwfs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsunwjie.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ibraiael.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bmykhsef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pinnxzts.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dutjlglk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3evrzbotp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3susimlca.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qzvpysou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bqcfdxts.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3soalsrjy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ftfavbwv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rdrtymoe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nzgjmmpa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ebfouiol.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wbzyfkou.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kzxjeais.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qmgyajsw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvronnjm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olssliyy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngbmsvrl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cexjnvwb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gypwmvzq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3grljwhdo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iofsrhfr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ipiddumv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gtulxpnk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jyiegazj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nfghmviz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tumtspql.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gxfcheys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbbonhex.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nbejeqxj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tztuuben.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kdtcyhpc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3blvuminn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eemsmpnx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3azgedtqm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ajkzdfxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uhwopijt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gssliuso.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xbyjfbsu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ksuxwcaz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qmhbagaj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mthelrnk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jahzkosz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcvatpe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3radazziw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kkfboaem.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bxjlfkgl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dltycebx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3itepjhik.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tyanpnre.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xsdfinyk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bqznunkv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mwbbdtxb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zqmbfclf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mnanjipr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrrbbkq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nqjuwhhj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nozmsjth.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mcbidwdt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxqxfjg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ohimikyv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kspylkqs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ybacrwzn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3emkinuav.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tbvoozlg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dnefrhvn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwxmrwz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3guduupwx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dcyijgrq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3sfgnuvex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3veleynfk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pjazgnlj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vcgmsxcv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jjaijrhe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wfdtnjgx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maolczfh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hoztuxqv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jyvlubdm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fqstjisk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ktlzwmuj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hcuxwixs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zgeaixdr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qwlqhxar.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mutohddv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3fcbeawdb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3exndpmsu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzlefbi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kcmdilcs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rdllygwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzxsgvyu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tsnnumcz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3safpwsgw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3prnmjqir.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkoajad.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nvxykdaw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3typbeskc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bzirovqz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tqzzkvgr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tdjcfcku.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zpjrgdan.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oouocbsb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ccfabzsq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3baijjadg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvnoftxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ynbptvuw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fwxhnqro.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhwcmpc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vxqsisuc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qwohxrad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdjdmob.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3azimsinv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vuejddqo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3caudnikz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3urgomsuw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ymxalpez.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gikjogxf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hqluwezx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhhftiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hpdstwpg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmyjssvm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bxnearxw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3djnnufum.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3akbwjsvj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwgwngfz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zclalzqh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wpqcbekm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3otznelpz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jgtewsww.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cumgabpa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dfukhbqm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vfqrhdye.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gkpuplpy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vnfbyjqs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ghpvupdp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3abeacejm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vbujcekw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oasarqna.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wiidbmyk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3obnojrgt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cqhvprnx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xexgjsvg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wceeprkk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbanbjxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tsirdjdx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vttiwvph.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qzknojyu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pdbulore.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3epvivzce.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kwhggxxv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pyjssxln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uienufkz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oceeksbj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sogxnoqg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqbebwa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkohcmf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qmwpuefi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjbipxwq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fucqhtev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnofnfxh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cvnlmhon.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3niskzsxu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wewgyyfd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ywilzhhg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tichemaw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dvzjqouh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubhisyqp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qleipbng.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sxhvwsty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hedtkcjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gxxgmyuy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3flsstyce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nldkweno.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kbmwmuns.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wwjtoksl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3selyprau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cbqajkhj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cqlkayda.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3efeiawsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3avkwvbfv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ikvpttnk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fyqpuclx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qaxqgatm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zyjaidgh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lqhlgjzv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ntgvuphx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqeadcvp.html


<!-- 参考信息 -->