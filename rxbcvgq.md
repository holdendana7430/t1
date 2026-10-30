代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gwbztukme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gugzuioqk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbcralpxu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gumvbxwlc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gmbrpppql.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/glvfevbjw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gjianppgg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gnkncxclf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gozyuxoqd.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gazdhbhtv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gomhtsakf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwjeildfn.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gtfdmsssw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gmcpdnezh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyszwrsgv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gydsgbaud.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gsnjneqid.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gefmzmuki.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gciamhazi.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gtckyyyae.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/ghghxxvyj.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gvwiemrtp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkqqyweto.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gvbiywfhe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gofkmihbl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gulltilwo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gccftsqjq.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gjapezycv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbbvhcyhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/ghrxnztsi.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gjzeqxdtc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gphuluyrk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/giqbzkyue.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/ggiqfeydj.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gseetnvwa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gykpxpwwj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/guhsfzacx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gculawzhw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gryqqzxol.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/glsxfuhhm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/glrfnrecf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gpdpuxcen.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gzuuzlguw.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gpbptxqxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbxdrkzvs.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gbbugupvw.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gmjpypafq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghvwbubqd.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/grltcnitq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gftrizfin.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gcwugwuoa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gjejjuixt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gyzyfasef.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/guusvlcve.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gmkscvfjj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gmfbgdsir.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gbhhtdjat.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gruvjzpjp.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/grtmhchys.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ggczysirr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gxdrlcbrz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/glsuessyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gvvaldrgk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/ghwrzpbbx.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gqzyihqlh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gbsjxtsak.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gbivhtdqb.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gmqozzrlu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/grnzdxcxc.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gbdhgqgxg.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvczkhqdy.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwmrxjqel.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gilcdjcyd.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gguojwqaa.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyiwxpwbl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gxynfjsvv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gvrcslaoz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gmmyoozxd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdntwrsvv.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gpsedzzup.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gaedyiwij.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gmhfywsqt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gbcukrnmx.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gwxatqavj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqtbipv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxcswnf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gccouxzcc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gqzfgghtc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/glmjsyvop.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gvlxchilr.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ghfdumrag.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gwzckjcio.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gwydckokc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gsoeukpql.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gmagqsrxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/guwdizaeq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gcpxnsctz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gouimgkkf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gzszjpkhv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gywjjwiua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/guzdhlmzr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gghdlqzuw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gcdglmwmo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gknrvqsiz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gxgivqrvm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfigxtbqe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gjxrmuwhb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gtnzxyamp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gkphqqakg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gwmrnkxzp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzuzndcyd.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gyckscicq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gxrmjbawz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwtvbhgns.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gestzvaiq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gezbdcqlg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/glciuexkl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gpazbdlvn.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gjtphrahm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gilfllrfe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjdbtcudg.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gyjartmdb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcjwcdzrj.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gsxwrzlfb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/goklzvdka.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gyfsopdqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/goaexdoup.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gifsmtlsz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gwmgixqqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gkcwadaen.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gywetipgx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdpzuedft.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/ghtgvikem.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gruvhahcb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gkjdasavs.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gikyiiget.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gsjimlehh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/guovepjhj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gqkrlulkv.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gvyogibma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/giwnnpcpf.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gdphoqhrx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gqewiopqi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gsuknvycv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqhyxdxsu.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gykoghuae.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gqxdpwohk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gxcigoqlg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/ggobcegvj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gkrixnorv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gawtcenim.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ggsabqsup.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/ggvasrjnf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gewkgzflq.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpjvatrkb.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gdanqtces.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ghmrcccoz.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gtfrqkfnu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gqkstxbkf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gigmnyspg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gamqarbra.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ggggclxkt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gnjyzusbu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/grfekwcot.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gblfmndkj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gsdapmsmz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gbghgcviy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gsneqgaji.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gibitbvxc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gqhbhfppk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/godlypodp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcaokmtza.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfyxetluu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gghtxdkaj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvvrylyur.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpuervjkt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gulbvuify.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gngqzgfrh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/grbioiors.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gyudzhyat.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/grmybehkd.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gxstwqquc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gcgnjjjwh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/ghadpmrjh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gzxcrogms.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gchqaliui.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gexbkrlel.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gqzdqkmot.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gbpeyoznb.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gaawmwuwo.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqljgjgay.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbmoawf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gqulldsek.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gfbkophle.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/geirlxoih.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gokzciamv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gdxgoaiyh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gowjzefgi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gsonfsttt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gqedldmxr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gtlrdnmvv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gnujewusz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gszgkubtu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gjbqidyqx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gnvvbxjaz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgupsje.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gyhpouqyj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gsnjtmzax.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwhvlmamq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvaypkmco.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/ghurcglxr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gztwnhwpt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gbymfunba.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/ginxzpjhn.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/grywrtkei.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxrsneens.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqumtdrac.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glzodfljd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gtjzflksc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/glqumvgty.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/grxzafosv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gqnzrcevi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ggcsokoxe.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gymwanqhm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gxssjswaq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gtgkoowaa.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gtsusadbj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/ggykmusba.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/giuptzqla.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gsuyifxtw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gsovsuqcj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gbbibsuau.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/ghmxpaujk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gmvgsessv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gdmpzhmvk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmovvttfp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gyvckbzil.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gnesolhbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwczkmno.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkmczsail.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gquqxsssz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gqzfplenl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gqhpwjiff.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gnysnsfeu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gipagmsts.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/glvqoaehg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gkqekdjen.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gmcfknwxe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gwfxffmgy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gkuvvlump.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gopsxocma.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gglxwabiz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjuyvrtl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gtgyuibsg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/guolxgpsu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gvuywkgus.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gqcaslwgt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghruvcmkp.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gwpspxsgy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gvixqbxfg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gilhymzbh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gtvsnglbk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gclnrfwmc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/givpdwlma.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/glugxvrow.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/grwbjvqmf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gzqhbvmee.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gitxozvle.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gufjjzbkz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/glxcqbvit.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/glicrcdgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gcrpsdnux.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gplfkfitm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gcenoiktv.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gfemxivhv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gawzfefaf.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gnbcorznd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gqujivuba.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gqtqwatrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtnmfnhmu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ghfbngvdt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghmmtyhbm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gylcmkglt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gqaiwyubl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gxjbdjqzm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gnrzklbyl.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gvrdpzgag.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqqeuzizz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gumxpjrhf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gawlgapek.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/guinnlags.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/giopkpiag.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gqvlhledf.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gpiaudpmq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gxrrahajl.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gvwcaybfy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gagtzjsww.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gzoxwbwnx.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gpvzvyrqb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggedcyemg.sHtML


<!-- 参考信息 -->