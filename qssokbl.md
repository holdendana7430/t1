代发 wailian999

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gwyzbdent.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gudfgqtay.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/getqpehud.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrdwyyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gpdvarlvr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/guhddazrr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gmcmuavzq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gacahynem.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gwqiondxl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gwsbmcphp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gmlqhxsen.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gcuyxfzxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gfhauuztp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/genixfovk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gergonosq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gaepgqook.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gtdybpuzn.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gxcdmbmoi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grabqrtce.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gykfrupeb.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/ggonlhzdo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gojbxnmma.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaaqzqkwb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gbmqcwvwh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gofxzdekz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gkaouqhrt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gvvdpsfdc.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gteevaosz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gfccalfpa.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gnuhgdhrg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gcvgcfwtv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gazyycogp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gvedarorp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gftploniw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gztxssizk.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gvoagzdlc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/ghoxvighf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/grwttebxm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gydqvtuin.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/grgqpqhqn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gphtwmyky.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/ggcreaewk.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/ggkhccupo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gpcgcosas.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcceibump.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gsbdvmbnr.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/giyjbxxrp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gcvpnnpxv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/guhbuanaz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gaicvzlui.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gswuxaqba.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/givcfzgkq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gdtmillmp.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gitugkytb.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gsupxlskv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfyshwlwx.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gwnfomekg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/ghpmotdhs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gviozoluz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gtbwegnwm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gysgscemf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gnhhezxnc.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gjrfeaisp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gvfvbzuvr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gixpjxliz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/guutgupzz.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/grqrwwvaa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gzffmlskb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbnflzhoq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gaixhjcvq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gnuonlloz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzuivowvv.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/grhdjmxoj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gonlqnhjr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gyppkksix.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gbfezbsoo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gmylitksq.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/glucveqbe.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcnbyfevk.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpndtzbft.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpwfvbnsa.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gsswgzuge.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzractify.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gzyxzpjnu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gngnlckyy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gmszwycpf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gqkcmrrxa.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gcnzovqrj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gqfqcbhds.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gmksjzxhy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gecvvacau.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gcipfunsf.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gphocpwuz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gxkdhuoxg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/ggkwluysg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gwcntqjca.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/grzwsnavd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gmnoyqwlo.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gfynjcvst.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gjjnsnsen.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gwwqsdvaf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gioopquzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/glqjqeaxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gowayctik.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/ghrhdzjmr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzmdueoay.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gmtmnqvxd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gwddbfhso.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gawzizgei.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gpsmusgiy.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gyxrforyy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/geniczyhc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gldrrodcm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gjutvdqnz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gvxelraym.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gszwkgenl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gkzkkcxjq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/givyjnmvn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gezraawwd.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ggiwnwfzf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/guugmkgfm.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwxlzlwws.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gqhfwjefs.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gobezdxeg.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/ggtiakanw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/groizkafj.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gyczxfnnw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/glkfxyikg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfqiwubey.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guehqyrqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmwduggrm.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gyitolyai.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gpsocqhik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gglldoemd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gpoeazjbz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gqhspnlzr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gemfxtnkv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gcjnzmsbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gykdjdkbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpfzcjcdt.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyxksdtqv.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/geyavkgpy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gjjshimwy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gumhfjzgk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gofsixnuh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfytczbgb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjcchqg.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gfdskzmgw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gwfhwfabn.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gwvjeyzbp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gygztdvij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gcrvlaudd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpoirzobc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gahtletni.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtyulcedw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/guoptulnb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gnjpcfefu.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gbvroyyph.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gimwptdek.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/ggcfgyevv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gnhwlayoa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/ghpdzkehg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gsvvmthxp.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gwwndedhg.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gnapjfstc.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gckilgjwx.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gmwxkqutp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gicufevcl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gksrkarkj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gdrbmhngk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gimugxcsj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gqtoqklnm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghuwrtfnc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gyoiemcrt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyuwwymrp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gdzsadulq.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gwlutbqdw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ggsasaltb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlcoqvtx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/grvphceft.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gswjxiwat.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gncfcisyc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gcybzndif.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghjklihou.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gblcnveoh.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gyuboggky.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gzgwpsdud.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goerrpmku.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gglztidrs.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/ghpawucxa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gjfwapmed.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gtkmdtnzu.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gkymxrbum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gxgudeqhz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gkaomtgsk.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gyxtihqfx.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gzbhzclje.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzrczyyil.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghfgkwtqo.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gkkfaxgxw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gjstgbkve.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gqyterrvp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gzaudknus.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gmdncfpya.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gvrvbjbil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gihzamjaj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gmhzerqbc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gwwcugkfo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqoxcrnow.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gsthjmghp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gxeukxwxl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ggolyawob.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gjpucexld.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gaekkxwsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gikowcnhb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmihpjtmk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdknielsj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gkhttspcm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gofznuyyc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/guczeeruz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/ghmmlpfve.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gzcvqtowk.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvabvlesq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gagbcdwhd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glcwfnaym.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/guotqchcz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/ghwhvoikq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gukxzkvqy.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gkyqixdro.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gnmhymmvu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gttjjsvmt.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqowfxlqn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/ggogxstsh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/giuwtiugs.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gqjxgtinx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gvqwtcwwl.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/ggabbvybe.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/grmnwyanp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gbusdbflz.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gucvwkefr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gwgsvnkek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gnibavktw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghjxhipwy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gynbckcfp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzgiknryl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gfedtobfd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gqrdnlsev.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/giocjrbqt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gqymqgjxa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gyrizwcrq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxislybjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gyjsizgpj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gacpwsfcd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxmlmjtlp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gdeuhmnnz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gbawjkicd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gblrfipny.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gbnbvtmzv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ghjxakdja.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gamzptfhw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gqxbmmxbc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnnkwsgcc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gjktcsuwp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/goqxmbevn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gtqzvrglp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gffqqjomd.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gufwvivgx.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gjgoioklg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gvysllgel.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gwbebwyku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gqixolzaa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/grhcxbfsu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gmpocllzl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfitrsggg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gzyvgoayk.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/glhkefthf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gtttfvisi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gcbahihag.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gsfkgfgcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzdghmsuc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gpkoibnmw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gaajhyynz.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/glfwxwvck.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/grsnmazji.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/guhxvcbpt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gqezhwbfa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gydxuqxzx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmjrzubnl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gyqnpynrx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfqpdgsze.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gtnunidgk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gpnirqolk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gcsotstkm.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gjwhrbneh.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gdaiyvwzr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gpojodzuz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gvnplyhem.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gygcaootg.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gqkposqjm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/giedffuns.sHtML


<!-- 参考信息 -->