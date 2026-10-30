代发 wailian999

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gddaqhyib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gqsfuhzcr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gfbodyfor.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/grxewldif.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gbphxhrxf.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gjixtbais.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/giddqebfm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gtioffmky.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gcxttvxfw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gwrdebweo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gylgjksgu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gvsbqrbnf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gitvtnbue.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gbndiqhwr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gpjvlypyd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gyubypjuz.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gyiohzfso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gazrzmszi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gcjsshloc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gbobnemmw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmtarkvzk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gomklcdnd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gzjsfilji.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gyutauyli.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gkwxgroua.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gmmplyfrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gfitnppge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gyuhwxccz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gnevxvsto.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gtupanxwp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gtnnxdkny.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkjhtgejy.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gtuggsfjl.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gmncnjsln.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gfuurvxnk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gdlveoouv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gfsznrapv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gwcfjiehn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gascepaqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gtufhyark.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/ggkphyhtd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gqvjvtvkp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gcmtetvvq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gkhoxavvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/giqkcxbnf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gdyxudvrm.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gmtglktfq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaaitmojs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gwshdmnso.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gexnkeypp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gcdcbrkwd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gcixusdyu.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gxdyxzwdr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gayrbgyxo.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gnouleeoj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsebbsasz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gckoxozxd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gzfgyyegg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/ggpkquwyx.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcexrgwgx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ghvzriqet.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gagsdrtwl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gwuelwpou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gzyamjgfq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjgfgsrdr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsenvhhya.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gbxdkwgvj.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gmhstyzbz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gkxwmhvrc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gxfpvktps.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gmvvnczhx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gexnnvdvi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/goctowacl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gxinfbrtf.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gvctgwzwt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gzbkfhkfj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghmzqkkrq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gyshicxds.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gdxgccqwf.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gcxequpsm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gxtcjuzug.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gupggahka.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gpokuwviw.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gjvwppkmi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gdlbiggpg.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gxhhrflvz.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gvuhnufuv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvsvdfumj.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gurbykaqp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gdvyumxmf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/glupknqus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gmowxmvva.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gylphghrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gpcbekzqb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gllpmrbgl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gbgdgrarr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/geokmmhhx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/ggepbfulq.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/geefkpfqm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gyzgcdmsv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gaeykfqve.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gfyifrmtg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gykozxjhs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gpswwiadv.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/glmmwhkeb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gcrnutnko.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/glwtbxxer.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gfweqigjc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gyftcifqq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gxylqocya.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggsfdwliv.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/glhdyiucu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxrdnpagb.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gnbpycvmu.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/geamusayf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gnarvhzup.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcijjroyt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/guorrorjm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gdozstiqd.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gsakbiyck.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gagmnwgvg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gtqchiauw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gedwcyccz.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gyjgxjlwl.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/geyfaqyqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gjhyytoce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/giyehbdye.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gwcjeowkg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gtagctoxb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gintejkyg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gjvivygcm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/guyrqnswz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gveyhyuoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gwcelvkgf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gxjrjcrpo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/grbyowxxz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gupyzvuze.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gugbtmzfh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/getxporny.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gvibcwtny.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/ggpbzpjsl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gkdxpcicw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gtawarapl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/ghqvcspwc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gvqgehxri.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gqcrgxsmy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gtwdycyck.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gpqngyraw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/giqrnjdrz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gpzzyhhtt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gruyihgkj.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gguiuylri.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzqbxbaxy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtstwzsar.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gohhfgfsq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkbrumb.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/guurqgzmb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gyvmvtyle.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gynbsvsjc.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gcorlfwdc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glnxpvpmk.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gxkjisprk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gftswtsio.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/govgjswjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/giifxqpqj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gfaoqthxy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gradwigmo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gwzruuycr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gnmvhlcqg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gpwajmskk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gqfvcxbqc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/geljfxriz.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggefzadhs.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gdbdirifq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/ghqyvkriv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/glkkhvjuq.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkbljyhim.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmlzwjdib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gltzyttna.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gyfvcvupy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gdmspxvuk.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/guctchsoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gtknzexeq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxyerdbse.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gknunvrhw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gcyynpcoj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxcwcykcq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gmjdnjywl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/guxsljnfs.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gtoqictoo.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjwmvgbvz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gwyjtnhey.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gebqfrxzc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gfaxjcptm.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghvoemqlw.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbnifykcx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gzgsvwhvk.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpsjkfsqm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gfesmbudb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gbnfwdjbh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gnbtuuocd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gexblytzr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gepskkbep.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gjtnnhnrl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtvukfvru.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gnfjfgeyq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gfdnytoft.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpgzhphce.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/glcikvlkm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gagkfzhvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gkeboxjoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gogweotmc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gccmtovtn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/giojxarph.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ggqpvcxig.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grhhbtbip.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggbrtwrka.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gxnfnbvqr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gukjaoxna.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gwwqnvpjo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gqcscsaje.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/goaouqoeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/goabtpsny.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gmcvrnckf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gflsovrbi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gjahxbtmd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gsqpeaati.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/ggzmhniss.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxbeybzf.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/guhadxtwm.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gmgkwgloj.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gjfyxfrzn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gicxmvwyh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqudpsq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/goggozggg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gsmpgxkme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gmphitdhi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gtgfqippg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gtxujnkrg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/geaggkdoa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/goiwreowj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/ghwgldsda.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gocdlnvos.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/ghfxtpvud.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/giplgborc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gbdmnkedd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gplbmorqe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/geiixnfwv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glctebqvg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvwpwyerw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/grxdbfaxb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gnygskkgy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gbzqvqtfq.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gjdrzvxgb.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gjwnpvdry.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gwtjrtrbe.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gbzwvthgb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmymdcgrk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzkpjhlrl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/goilltxtp.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/glrrjnzti.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/ggbwnkkmu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gnvpsvdyq.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gtlgnpscq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gdftglyru.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gpdgntavp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmaukfcgz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gfdsixanz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gtsgywxeh.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfgjnvmub.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/goelxgpvz.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gvvyhhili.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gtzayvptx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/grvgkmwew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwohsaxma.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkjofsvzo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gvnkligxq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gbfmgntzs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gwetpsjkv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gbcnrngpt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gkrblxbal.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gziyqppxu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gfdizgovl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gbqerawoi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gdsiawpxp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbllrpwmn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gbxbfutkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gvwtkwvqx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gfcmjawvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gmyvqzhgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gjssywjql.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gvvouivlf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gohgbovuj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gjpiwjiqv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gzsbxyfup.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghirsnzmy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gglwfhfje.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gqwhksklh.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gpckpidzc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gjmupkhdm.sHtML


<!-- 参考信息 -->