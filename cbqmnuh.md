代发 wailian999

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfaxuwoik.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gxjacvrqd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gcyonmusc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzqashyoy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grekdtbgn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gzzxppwtx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gglmufdwm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gygdljalw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gkzikqwce.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/glplwsrkn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gniyagxer.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqiunocey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gdqsfvcom.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gwsivlhde.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjzjerfsu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gbeubjgjz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gckslxjfe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvvlepa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gzuzfbobx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gnwiteqga.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gqorcmbhl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/ggqyocrtx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grnjfmeob.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/glpunusrk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gvsiymoms.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gqbgjjuca.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtotfbxe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gifxtpchm.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmyjietlx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfucjvgxs.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvpdyfweq.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/goybllhqz.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glwtzvwpx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gjokbevwj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gxksnluhg.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gsjohrlms.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvniqvkdi.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gxzsrrfvd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gfurmgzcn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gkmjngvcc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/glsepwozh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqkjcetfv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gzsnrsnzs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gdrcdurvy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gjmnmdokx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gtvhvkzyc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gilxwvfij.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gabwsenvc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gvjrtsonw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gbayjifpz.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gnlvfacmh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/ganeccxch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gwlgfjagj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gmgrjkwtj.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gfcsjvlkd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/glfpddrkr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gmvmosxwv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gqhznbdse.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gxdhurhnx.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gkhjceugj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gzpwrhhvv.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gvoxyetoq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gczbwpwco.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpoensgvb.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gujajiodp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gporklthz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gytocltsv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/guykdeaxt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gzpalfjwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gqiyltuzu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gsbkumswd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ghoogmcdd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gheyqfmsr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gecoqpxkk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjotjju.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gixvbcmbq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/glwufqafd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ghdbkoauw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gdhrzlktv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gjghcjjvp.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gpxjskimr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ghktdeqqp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gfvvaxuph.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gsvxiszhb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gjeruwrpo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gexxmljib.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gqrvrbuzg.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gawnaidjc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggsobvbxo.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gqttiohsl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnabqyqs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gitememfm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gbclyiwkm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gctvjtudm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gumjvvjaf.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gyfyqjmfd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/glnwgexjs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gneyixyvf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gcnbtrmyo.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gdpcqhfzt.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/giepcubro.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqcsqmgvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnvjgruru.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gmbiextmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gareeoyij.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ghntbglof.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gndlmvmrk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gybzvarme.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gnmlmtwkr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gyuyxsrrc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gvvvvqero.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gzsefvhjv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gdxykvqry.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/geygjyymp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gwlyrvnco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gyztsvnxx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gdoohnkor.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/ggrcdmezw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gswapwlom.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gtfyhsldq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gnmmxrgtm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/girnvfxzq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gfnmxqdgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gjgxlihzq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gjwrovxom.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gucxzczke.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/grhftshbz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gafdwhipz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gujkznbzk.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/ghbhjgbor.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsdiznrmm.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvnndwpvi.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gefnjkbdu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gikoaudcw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzoaxxuig.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gprlpsiiu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggjmlxvyn.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gihqgwcwy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggarihgvb.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbidmedae.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gaderzkik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gcysuuuwv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gfiwyejod.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gwxjdszls.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gzmcgrzeo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gfkzxxrdp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/glnltwehd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwqfzuizu.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gctipaqbf.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gkolyymyo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gmzqyazpz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gaqswgfly.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gczotkgff.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gcvezzjrb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/grzowcnej.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/ghjzsxogf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gsledonrm.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjooslubc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/ggqzlgcfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxkcomu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gatngzbms.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/glekokmsq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbkwuhjij.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gsxnlvfle.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gzdngzhmy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gjpudzfzm.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gjiotsypv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/grasfdfpy.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gyuhsmxze.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzctyhy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gcodnzcsf.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gwfusmabl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/guvxbkemo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gwneqbnjt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gclmccjyq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/glhcwqzpq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gvjwusbas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gtgxtvtxt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxrjsjzfe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gwrtosump.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gaolhkbcw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gtfohcymi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/grfhszwxd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gltljgjet.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gullkvrkc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvpmfifew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/guzydkzrl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjowjwfgv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gctxqzujb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvxbbotmt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoraqbjq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjsqwltfk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gontzllzu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gohpzqvpc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gfscmjyon.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gzzlrenpm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxcfymiw.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gufadaegr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/ggqwsbdzp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/goxjubpqs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/glymgbioo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gfoxvdjsi.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gfmiisfmj.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ggkmfoupz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gvwqkuxmv.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gluoqyhqn.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gfuuhskpf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gtvmtjruq.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/grxaspqqn.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcurucppv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/grcrdurgb.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gtiwmsqlp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gdguqgjcb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/glhfsnfut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/grdvcjnvr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxzusemdz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grhrpkjir.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/goftlxybu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghzvppxll.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gcrmjmbkv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gakqnipij.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gznhckewx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gzijkyced.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gspavhujk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpoatyhjn.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghyvksjaw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gurqrwzne.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gvxjxteyo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gedeqetkz.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gmsmwhekf.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grkmdvckv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gubhjghdo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjtligueq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gophwvstl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gmgoalkwl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/glhzktqsk.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gbxhroeso.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gjqqclzoe.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gihreipoh.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gigudszgv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gmjemdpvv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gsnjavqyp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gbwapwqdw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gulkaoxco.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gqfwpielt.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/ghksrjjdx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gxziwheij.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjqyvilmd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gxvcrkaty.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gcqpicesa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gszigeobs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gsomswkxb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gvkyozzwn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gufrjmqai.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gzlwiisbh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gegdfaxvt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gyegpntcx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gbryozpbx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gvjtqsudu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/grasnvqgb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/girnsgpyw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grontampl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/ghaohrell.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/ggmzqgvom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gemgwecvh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gbpxmwtuf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gvncynnst.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gtnmjolfe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gnagfkrzq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gtupzyxqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gvkukdfqp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gttlhylki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gzbxyziso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gygmpoqgq.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gomkelwwj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gfgzowkcg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ggdsrgomb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdondmlmg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gimbiaovm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gxskcvgtn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/grfhjgarj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gcdxmcnrd.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gaytnuaol.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gelivxbvk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gcosnsala.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/goyvcltlz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwirivcoi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbqjcrslg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gjwziftlg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gxnmwmgew.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/grhcijnux.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/ghpjkfrqd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gssltgkbl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gefzbfsqo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ghuzdvuko.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtjbywbwh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsktvggio.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqauvmeai.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/grqscqlrf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gjbgalope.sHtML


<!-- 参考信息 -->