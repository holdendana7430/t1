代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gzdbkihzf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gihuxfkzz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gqyrhgzqo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/giqbrnobt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gaqyjokhf.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gvrfaolch.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gahtgbazt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guonztqtr.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/ggddkwwcm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gfcmsbbmp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdwwwvjyg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grfpdpmmp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggfkprxne.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/ganzbzchi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gponrracj.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gnirqloas.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gtkawwzca.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gnsxmrozz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghaojhxrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqwffsdtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gornsfumm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjtwweaxl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gmedxbazw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gycqgmlrp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ghdhycwdm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gqowdghxu.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gkidswoex.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gpinskuuw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfnzxcxfr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/giaeobhpq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbcvhbgbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gzutojkqs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjoouueqq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ghccyyfnf.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/glyzpwlpc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gqxdaxcot.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gyrvzhvpb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwiedoqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gafxbfhzt.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gjnxwfoyp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gekrhsfjb.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gcrngpxtd.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gocdahnvw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gndusczdj.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gaezviaej.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gerqplayk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gftmwecaq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gmmzdhixt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gikdajqjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gvdgrssfy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ghinscsui.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gzgmzsxdw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/ggxttkshp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/giowplfyf.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gtwabhpgs.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvjfoblqy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkqrtwtwv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gsfkbnxqd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gfgaovnsg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gtqqrsitw.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gjcfyjqtd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gxpplojdd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gzujycbgm.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gdqrpdrhb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gczfntjeg.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghqnixlfr.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/giczfmbvr.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/galvqfqrv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gghgasyyh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/givrlolmo.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvxgkipun.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gnhfpoalj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbobmwim.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gejtvqsur.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gfcxlxzbq.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ghfqiiewg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gesfsjebc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/ghqrmzgfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gzhkgwynh.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gigcodbdv.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gcsncvywc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gcjsrjxae.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gvsdmgeou.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxatiyfzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ggfwuffph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gpjvlntsf.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/guuixzbhz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gojycwtgs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gumrnvubh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gdniitqpz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/ghwipoztj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbpipruqd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gqgciugvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gfihqrskj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gfiwnkeuo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/glxnnldqz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gsletpwhj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gyvdtalki.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gexcyxhcg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/grqwjggeu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gotnoogdc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gboqqetmr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gtueefbbd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gtthmmkqn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gjnxvmbqu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gusbwxigv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gnppruvtr.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/geteyjgbp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gabvswqcm.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gswpaakve.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtjsybmqj.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggbpbwwjc.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gnigxbgdz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gaipefqtt.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjcjzeqhh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvueeurcu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gplaguwux.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gjfowdrmf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gerzrhpxe.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghksfjfks.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gnwslqnph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghghuytkf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gxlahptyd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/grocanttw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gqxioddlf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gabbczyzs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gtzoiceqp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grcfpgdes.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gspigbtkn.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gsrrlahiw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/glazvblov.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gvlkgpsla.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gtmcunisp.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gzrlzkqex.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gglkpyphb.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ghqcrkhjd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gfqydsrmj.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/givfevrux.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/guxojipyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/geqfzhwpq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggnnotrti.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtvmdnsgy.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ghbxijirt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghcusqjlc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/giywknzxw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gxtaomczx.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gotdtfzho.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gxcpzurow.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gkacebfgw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gblraxkfj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gxtqmauik.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghdtsbenb.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/grgzvbudg.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gghczeudi.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbbctbcbo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/grcopcxaj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gnqlacxik.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ghvlyfuep.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gmyslgrdk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gmfbwlufz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvxyywiaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gytbslhbw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gtxeqalrg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/glhrsjlxl.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gjyzikobp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gmyawhbyx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gxaptmpzu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpzytyuov.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gouxebdxc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtyekrfkz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/ghvelfhbi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghqwaywvp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gcsdatueu.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gkwhilibj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gjqctaagg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gynfqinhq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gmawbcjgn.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/ghuhokjsj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gzgriexox.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gsqjcjsjs.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gbrivaowq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gkfxehezt.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gufsswqiu.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gfuabtkkh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gzpjijrpw.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggercnmxl.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gehjgtbal.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwcrzicbz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gryuhqyko.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gsargesgk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmbmyszya.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gmxvsdatw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzaksxdeq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gzmdlpwki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gfkpgtqen.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gghbxozzi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfbmrtvku.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gqucinscf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gwgsuqdgk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/glkvzeqtw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/guocbfhbt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkslacqzw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/grisffkqv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvqhhchmb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gorkaebri.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gqzsjfayo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/goqkwdnjl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/grdpmpqlg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gmuodbqmw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gzjqhrfcn.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gupokcsiq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbgjivjku.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gcgeeaclz.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbmwcrrvg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/ggfampmar.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gpgphevso.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gvyqosnyu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkqwyjzts.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpadfstxx.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gumjndnku.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/grqfqzvmc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtaonsekg.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gvqgulniz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gykmdyohq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gxvghjxzi.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/glzjozdvu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ghlwvmnbp.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gfobqmayb.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gslepdzjw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gzugzmozs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gfcnamfou.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggprjznsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdgdgpysr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gskvvwjys.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gmgbzrpre.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gzvoyozcj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gylbgjgeq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gfggmiren.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gcjchynkn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/golbeista.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gmytxvqaz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gppqknmlt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gmfgvfylt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gknubwvgz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gsljfadxd.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gsrunhosy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/glwwdwjzm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gsxfuounn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gmsjrgdlw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gkefknjhf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/ggeznkscw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gucjmrmxs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gjhbdhgvk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gejjxxdzy.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gfmvorxpq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/grkhqyago.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gtqdsihss.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/giyxaakaz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gfkysjovi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gktruljqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gwhhidizt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gmlrnfisk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gdtsgcrge.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gpuxdmggd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gsvqnlran.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gvzkaoxvs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gqrtbhube.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/goxfqsnfi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyphjxhn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gbceadgbb.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gqcsvwlmm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gmlebbxcd.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gpszkocan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gheywrbjp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/grffedxuh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbgmovfsu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gasendzvk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gglqmnswf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gdhwfphxl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grtbedhkw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ghdmtorcc.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gfgyumasv.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gfgxnrkqj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gqizqgtow.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gneuzgmdp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gvzwnglzq.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gwchoukms.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/goxmayopc.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grzxmeurp.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gcyibbaoj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gzbostgnl.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gqwliheef.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gyozbajij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcmllznhx.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gepgprjee.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gkkudotac.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gayigikdw.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gmserahhf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/grpezllfu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gnkltdqyy.sHtML


<!-- 参考信息 -->