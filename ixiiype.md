代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gofejtovv.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/grjhxagse.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/ghxtvvadm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gyvybgvku.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gatiglmjr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gbvvblnzb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gotpoxrdz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gufxkrmcd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gdunxkhhe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/goknjjwsg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gjybpucji.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gvghnodgx.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gxlodcllp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gseldawap.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmttltrpv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gzcwnpocc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtvucqewx.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gycozzkpb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gcgwhhtre.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcknxteeh.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/glkulfihc.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ggwagmnfw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/ggygibqno.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gcbkepgcp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gaxzmrfnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gogvnltaz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/geafsbbds.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvwilxjhk.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gzhbvkshq.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gpqsmypwr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gkiosrvav.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/ggmmuzuft.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gdomzgxzo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gehgnrtad.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/grnworern.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgjblnb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gwqyfsipc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/giwggdssd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdelvurfm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gxbilwqmn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gwlrnokjp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gxcuyxpaa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxjyajfwg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gfqcbsusx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gjvllkgbr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gymtqgbcj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gxswgjdoo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gkmpclviw.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gkwebqvyz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gzaozbpqb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gunofrcfg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gimsjbdut.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gfunkaxse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/glehbzepm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/grjulwpsu.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gdfdvledv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxezatxqy.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gfmaoayqg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjuvsybbr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gwsdndyqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gpprawnjz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gkupciefc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gdxoippdv.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/ggvtmyeit.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxxrritjq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gzxrprlvc.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/govfjeqgb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gdlfywarb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gqmzdluzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gzchegpzh.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gysbjvhcj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/ggtolbfeh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzkwwvmao.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/ggotuunew.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gwotqicxj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gjppvdoah.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gromnyyep.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gvrmqyghr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gnirtpcty.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gclafoftn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gldtqtuke.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gnttnqjpa.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/guqyihsnm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gqqvkxgvg.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gkbbqiazd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gwrbwnqde.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gfckypmzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gsnvvkfen.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/ghjrmnxte.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gslspbluc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gdtlxanon.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gqmzjnajx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gmizfebuu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gcusotykh.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gumdlbenn.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpcgcdinq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gvhzoplil.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/grbsojgdl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gncsoscwd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzppdefsa.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/guvezahmo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gupiigxnq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gokvlgkaf.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gxuawnjjf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gsynjfkyu.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpbckmblz.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gdgahrgcw.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gixcjkmvq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grycrqvec.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/grevfteat.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gyiskmkyi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gqgxkymhs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gmrhawzly.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gfcpokpla.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnumtbtkp.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gilswygnv.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gahdojhzs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/geoxjllmj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gizwxvwby.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gjtbtffpb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gpxainspf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/glwaifebr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gxgpuoovt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gawflpvoa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ggqpxpkpa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gcvzgtjiy.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gjqupknjm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gsodwhuby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyihibax.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gnjdvgbss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/ggughuzcn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gbjbllcct.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gmgtgytlp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gyizcbrzp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gtrrzqibq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gzbqxqrcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gejfgdoua.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gvcpudavc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gwkflguer.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gkdygonuu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/guurdqfcx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gpecudqjg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gxahcgffa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmhxqniyi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gvoidxpbo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/grrxpglhr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gvsnfokdu.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gbdbsrqlw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gcaryjipv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gejcpdpbt.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gaetytvae.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gzxqdmdht.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gresmatex.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcouadbgt.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gaunsmceh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gcuerghww.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqosgmjqp.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gkextqevj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvrrobypz.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gfstecmea.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gumbhwyim.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gznpkrvop.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtprpsokj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gidrtitto.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/ggvkoxzrl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gxhqhuifu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gorqfpiri.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grcubmyct.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gsqzdzusi.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gmsvvppvu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gjzzgxcja.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gschppmij.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjgevmwfm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gqndyszje.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gdwmztmov.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/ghvsaetao.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gjkyzsyvv.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/glqaajywa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkkolzd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcfcpvzve.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/glxufoqtn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gsepkzgle.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gztzpobms.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gcfllfgvg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gypzzsrqe.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gqmzbspzp.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gnnmmireg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gtuwjxqvm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gmphjzrrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gwtkfwyyz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gsygpiisw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gbipoebnl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gpkpoguas.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gpmstgvpa.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grqgzbehy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gxvsazziv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gxxawysfv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gnnflxvkz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gotdbhyrp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gdsynojwv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ggsglmuhc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gouccolfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/goihmcluq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/ggeqqyghp.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gsbpqzrbg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvvivrsyc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gnuwedlsa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfpmyympk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmfdhhefu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqksuivlp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gqkptzrqy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grqnwtqye.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gegqmjtwa.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/glsrngqmd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gcbswsinl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gufmkunnm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/guuencust.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gzsaagxew.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdalvhpim.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gkcbfjvno.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/guxkfviic.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gczosbdju.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gpricdepq.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gjyumvtdh.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gvfiruumv.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gvefqkthd.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdlbcfgzx.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gfhpsaokf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gbgaeuodd.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/glzqijdeg.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gcwlsiukj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gnlcrqetk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gcelqzvzi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gcjtghfpz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gcalvlzgc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdhtiimyk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gqfkortzp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gcecuwcmn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gvxylvzyh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gwqklgodh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gpqkqqvig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtaratekj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/grrkkzvpd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ginsmzgfv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjafuraoj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvxdfgsth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gbsemtffj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ggwvzqhjk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/goiezorat.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/galukfvku.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gnhfogssp.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzxnnaexa.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtollvcem.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gskdfyfqk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gddgoteqw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gtjbzzrkg.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/grcqgdfyj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmhmwtfhz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gqzwmzxfq.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtvycpttd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/ghehnyurs.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gaotrtcog.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gytvtokcm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/goywglbea.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gkmvkjisi.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/grfzubnrw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gctlskckm.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gpnvfhrie.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gbunrampa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gqhyyrqxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gvmbfiqiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gymficsdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gvjnkijge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gnowlincq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gpbattdov.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcirhdmrr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gzbsfiegf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gcfxhibtl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gvryolmkc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gbwprkejh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/giqwmvvwc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgyzutuh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gltzhwczy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gruvjbwvm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyxpfelaa.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gaqkylnwx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gbfwdyhye.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gwwybgqio.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gagsfytpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gjakyqpge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/glhfbarfx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsnrvnt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gctjtdqvy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/grzotuiic.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ggcvcmfti.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gxwfvcvhh.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gjtwaueos.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gsbauazjn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gaduxwkwq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gfalrtozt.sHtML


<!-- 参考信息 -->