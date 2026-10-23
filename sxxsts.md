代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxiqbhc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3odngqcfj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zetuifdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rfarxtus.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iihdxxcp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrrieco.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3psqxdzdp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkolzkgh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lpttuvtb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dctpwmgx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nngzmnws.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3aecwmlxk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qdofaihd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3blwqdzmt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scinobbc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ehflredv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fezmgmog.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dlpdhesh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iofbbgpv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjwzqzou.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ubebspes.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3swccqymo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tuvhhpxc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vaykzppr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kpjjmedk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qnbvizvo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cniwcwab.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jakjhcyl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fjzisefw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jmddpqrf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3soapzcvp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rkjisgbt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozhkwvpl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cxnzmpda.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lozccpkw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qzbjvnfi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fbpflykm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bveskbyx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mdeubhoj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvurkklv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dtilphnq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sowtqetj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxwdpa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gkulmiho.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swqseajs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3syvvufsh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jqahpwzt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qbzfeayr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jxgqfdfm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3eyobphlh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3trpgpszt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dcpcqope.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3adatkstf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kenexjzc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xevftefe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kezmmtow.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jbtvpzyi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmyafeuk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3krpxecjp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ynivdcfg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3enppshgm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aazyfbfr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eyocmlyv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mniefprx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tzryxlap.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hodlrfib.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnuzgiuv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydxabwsd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ietiwcha.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ftmrrnow.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yujhisbq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sznqijtm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ivskxxlr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lmawcjxu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xlhxvujm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zgghwknb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzijznkk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cohiijhc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucrhepor.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cagdpvee.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjfnnvv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gzwkmtqt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gnrakgle.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jcdkbbhv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3afzaoaud.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ahwetdjh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkjwwpf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yfcokoxc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjufkde.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pibobyop.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3aqzkinan.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3opqvdckf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wandowpp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbydlmb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3azooxyeh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfatthqt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnaiuyxh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ppfbonjb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cnwicetq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3empooulh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3itxlgprb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ukzlkhhs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cygvllba.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3klrgqhto.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dbcxgkud.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tunriwxq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xwyfwflk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwbyjen.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cilbuusq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tiyvzzfy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jmeeindb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zddbbcdh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zyrytcar.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvpggld.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sluytlts.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihwdtgnf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dxoqztqm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cxjawrbe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otowncvl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucbjwgat.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3drmiiwdf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrucmtco.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qajkrmlh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tonrwrcs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3txhzswtp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gbdppeze.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yqlzscyf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3itxujgjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytlnfgod.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ktqmvvaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pygwqocn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkxrrihd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zvypzmub.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3votmbmca.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihxxzewf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3extebxry.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qoqcdikp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dqplvonu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lhdszuzs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umnvsmsm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dtdugsbg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pfdvqego.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gpaaneau.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijpttkhm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfszakgh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odahafbp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sciigfiz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3msopptwv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bzmtrmji.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dacbievp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bktfowfj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ciotyknj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3utzusmxw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sammpcbn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vlbwgoha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zgyawogr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hbuqiiae.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlpbsqmg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jddpdvgp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vtmfmchu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mtegfrhu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfgcemh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lzhnhegl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rrzizcvj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xqeqjndf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wcdhikqt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bwxsdsav.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rvauqeto.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xwvvrnji.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bxxnjaal.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qowselsk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3medyqdif.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xqtpckyo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ntutqdca.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wydjgmyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wcuzfelv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3csvhhttw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lofuxnyg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gzqjlaxz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hesvdyoh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axegpsfe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aouqcjkq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ozhzmipo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3avhtvdqj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hizohvkj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gyhehlqj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ejwysygj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3swciasrc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ejitqqps.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vvinemvj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3abpmdpbq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3julalkwu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jaerwfdt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nhhuqdnt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mwhtkdtm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3eomkfofe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3krticpbm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3frettcrf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3khcjvyfj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aauvzchs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjabkkpy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qhyheqrn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3oarvmkhq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wdngzotc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjivronl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ozqrovpo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aezpjhrt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xwmoorfx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mfoumdzw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3algsllyx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vrbzwgey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hkwnrkvr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxpehb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctcbuofr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3voqcuxnw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zbnahbyi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3evjxapki.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dtuzxbnw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qocrlscl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ypxgbxxj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3eikmobim.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqnkzfot.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ocvokcig.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zbocdnnv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwpockzz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uidhhytx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ktdnsqnk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hjcejxrk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fgifdexi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sqexjtok.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bmvjjjfi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wcnmqpzx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dnkfregn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxbbnpck.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3shvmikoa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ieydvycb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3apnlotyb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wnrstajv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ufvkooti.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hpggypei.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qizjjzto.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwbwoqcf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vmwwfhdl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dzymszdg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spdpgfyp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wjfqnzvr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3oauexdsh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hbopzhgx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qkdlvmwd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oprqynox.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yjtpypgo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyspxuc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3icuxmlla.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oufbqwmm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nundxise.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rufxdjbu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3luekyrki.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mbveghip.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdqszry.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmrmpmva.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rjsirore.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jxkthmhq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pucvkxir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3shvqzapw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3iwphfxgj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qunbytdh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hgqwohgd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ibylstsq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ikxqpxzd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wypohyoe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nwflgyyg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgauuxz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cnwcjxvl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3axjajuyt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mcebzamb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xywcynqj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kcxbdjzp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vpluaagx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqmgucb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rvmavkjq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szmxfhyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qkorrxur.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hnprgpbn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xxfokxfv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jwmhhgrn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yzgbiaky.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tspehviy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3whuudrlz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3miivvgrw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3whlrtunf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwoetxk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3utgzdkbp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yipqgkkd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qkgzmxcf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ttnedimf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3natlxixc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tznkjwic.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3naruccmg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dxgxbaat.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xhgdozpk.html


<!-- 参考信息 -->