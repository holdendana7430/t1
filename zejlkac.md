代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gqwwmgqvf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gdjodujng.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gbqwkhsnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gnuleyzzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gopmbradd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/glovxgopt.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkfnujemm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grofxbsfx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grmloinhw.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnjrardyx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghxfwunbw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggskoccke.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gcozitggb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gjdwtdlyt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gqiccxatk.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gfprojpmz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwrhxzdnl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/guonxwegu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/glzfmdelj.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gxkpllavz.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gsqarcrpr.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/ginfwrdxs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkvkzdogh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gbgfcvfmt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gzskssdfp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gkyvbrxok.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gnkbtkcul.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gdpseslrg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/giwpjxdqd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqxirfdj.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gavkvngxy.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjuliybbd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmfqvklpo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/geabbbcqd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gwuocjpcm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/guukyxqxo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gpzvouxnk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gredxgzap.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gnhjjnooq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/grzdmyvmw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gmlofdfya.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gbndtbutm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gcuvmzqae.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gplubueje.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gamoacwuo.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/glpljcpsv.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gsnpvkpyp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnhwzvgiu.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gkwlvcnha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ggryomusx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gxcdkvztn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gjudxmxzp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gvnxinwgf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gbfoikdhz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ghjqwpbhw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gftkytcnv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gnromjmrl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdgjymjod.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqelyhdgz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnmqibxdl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gdpubkgnk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnumhxhre.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gthaplyfc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gjbluiwmh.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gttmmlwee.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gqwvzzdan.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gkxrbnvuo.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gedxrsuml.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gaoiwejjh.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gohrzfwzi.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gurvmazll.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmnwava.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvzstdtcc.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gvoqbtcml.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfgdpdhhk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gzjgoyoqy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtdvlihhi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gaozqcfok.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdwbeyjup.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gwrfksjeh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gekawqnjb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/glsafbbce.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gnxwthien.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gfiqyzogq.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/ghxvwgfqf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/giinbfzaj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gqysrmdbe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gptmpdgvc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqerjeton.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gylpyafdm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gxafdnjsj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzwbrbd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gxbvmbjvk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/ghxgillfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gdjijjixg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gyduqtwlh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gyhqvxjnq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gumkqcppq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gfmrsdnyt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gbrlfchwa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gzaxlyjtc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gcvhmvvhg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gtvubhcah.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/glazmzikl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/geemkjkde.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gmoyxatzu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gpkkolhmj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/ginaafxse.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gnfcuyycm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gyzgrqbfv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gfszgedgg.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gyrnnwtvn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gccgqsqiy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gapgpboyx.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxuahwvny.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gptilyvxn.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gqofsukxx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gyxxlzbxh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzitykbei.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdadizwip.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmsbmbves.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/ggizrqjlb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gadwidirh.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gigwyyjuw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gxmloxuhh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gssavnthl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvzrtwc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gvjpyiafz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gcnnzcbfa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gyraaoxeo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gafsnltso.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzrvpqita.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gcdbjwztr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxmesrcpw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gaikryjjy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxmuylymp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gnebovjze.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/guedsywzp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gagvmwwqr.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/goyzdqyex.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gegpivymb.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghukghtbn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gcfkipcds.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gwxoxbnsk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/grzmafsxk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdwizdgst.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gcfssuwvh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gbpkyauuh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gkywvihro.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gyffcgcrf.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gntrvyrpv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvwoikrqq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gqkddhhmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gyzmfudbs.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gnirypoqq.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gxvpweiwb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzbgmxkog.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gltdzzkgt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gunlqqqlo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gbtkdczly.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/grlqrltsu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gwvddkzxc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gnsuwdbqh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gkcvyxurq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gyndsiczh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gsbltrlhh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gtnmrtcgp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gicoogktp.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gnquallrc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gokmxmrua.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gtzvykjlb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gntpuxxlg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/giihdqhgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/goyswnogq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/goqsmmlnm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghmvtdfpe.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxothsegw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/ggotgwusf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gqjleluvw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gypfdcpnz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gtgndtbev.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpmbhlizv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gopatseaa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/ggjknifku.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gybjtltoy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gfldqvnud.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gbgmmzzxj.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gseghcnxy.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/guwxflxqy.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gxkqmubmp.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gtwgtphke.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gnopcnctd.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gjyvwnhyx.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/glstpalsf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gbgubucsk.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/ggiewwkcn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/glihfszki.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gvauhnewc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gvdeeslch.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/glkthfpgz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gbzqaquhh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/glsxrzlhf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gnoclisjz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfrfzyzfa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gmxcghtwg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gqlqvjzxd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gjjrgwbua.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvercjuct.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gwtmbngvr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gahtuzkqv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gchswkdjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gqhznxpub.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gwpgzvtvx.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/grvxddxiv.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gznvjnrir.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gktfcoakn.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/golglsnpv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gwjiwxurz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkhnhqhks.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxnjfdvmp.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqzfsmzzj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gkvzvjqyn.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gmydfpcjl.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gpymuxuea.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gvqkoexlw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gqnayekwh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxhvpeqdi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gjwzvlupq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gtjeymcnb.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gyiimjxlp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gibtcbrxm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdaludgop.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/ginymlbkp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gutedbifs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gdllwvhvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gicekjvse.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gwnsakrhs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/ghobvcnjx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gslgnvwcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gyftgwvfs.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gkrjodurk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gevraelvu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/ghwepmwjc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtefzarwi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gnwfpolhq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdgxtfzzn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gbnwrgbvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/glmqoheth.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxwxzphq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ggicmwzzq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gpubmzkmv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/grvgenqbo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/geyyosqle.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdhmhzzoi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gyipiisyo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjrsezyms.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gotrmzzjx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gbccoqbmb.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gblcxoxam.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gijosgyqy.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ghflyjuik.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gteqdzzxt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdwsgmvud.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/ghagfbvpu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gucpccipu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gnwmfzolq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gfdobjtke.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gawtylbyy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gzkmqvdmm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gwnlaifxw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghkrleyjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gzhijonaj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gndjzehro.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/galdblsgp.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gakpyelnl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ghdagqjfw.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gqygnepye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqyktftn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gtycllrah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/giqwqmuyi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkzvccmms.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/grbthzuol.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gcuqqmmqs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gvouvgjam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gpnimrjoy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ghlcrautr.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gmspkqkkc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gzklzvceu.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gqhhvqyvv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gyzkywcsx.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gporglyih.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/glzsotudy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gogdmkbjh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gwurspvka.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gxesaeewp.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/ghblojmze.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gxbwtmgob.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqombagha.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gwzedrwxg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gcuoscgwk.sHtML


<!-- 参考信息 -->