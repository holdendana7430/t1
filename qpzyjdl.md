代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gjiexkhzj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gadmfthvs.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gqagclkvl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gzsltansv.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gazsgrlno.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gyltqjerz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gqrawohxr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gcazfpdqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gqekqduvh.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gpzmnssej.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gewjowfmz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gcneyujmv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/goaojnhvq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/garagebyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gxxltjdij.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/givwtuipx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/guebjwsri.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gpmuwokza.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gwbmaztqp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gxdfduiak.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/ghjvotndn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gkgfiutix.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gupzsiquw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gvdrebong.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gpehdzvcg.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/ghctxebwj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcyhcoljt.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gfzyuhqsk.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gpdbhpbqe.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/grpnjszrq.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gkklmldcf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkyizavlq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gyqlbgglm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbljxcadu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/geukgoxlh.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gygtfhzgo.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gcouuequj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/ggnfkjnsy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gfjvxfzge.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gesgyxliw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gxptkabos.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gihmwtplj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gfliewrxn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/ghgvupoau.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/geosgbnaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gakvtxypf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqajddbjb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gnktmzyee.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gzawwspso.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvmmcnjdt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcbqvcxyh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gzcapwezz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gekjwvvuo.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gbndqnkky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gcrkpmjsh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxaqbczoq.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gwzhrozob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjtyyuiwb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/glasrdqzt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjxiwipie.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gvbfgflvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gbhnzpzpy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gwzlxzsbw.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gasaiocgf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gkbuxjbob.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gnetkeaol.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gefbcdqxn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtiahapcr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gjrwdsueg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/grbjqbiys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gnvymklrp.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gteghtbtu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gxqtgwwcj.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gtwrhiwjs.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gmybgrsln.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gzenofqbz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/glawetvoy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gnawkcvdx.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gaqogesjp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/glfuaxesw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ginfhydlu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/grtmjrmwj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gwivrxtgv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/giwqntrzl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gpjintqcu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gvsrprklx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gkjrjdoop.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gwfnbsznw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwtmmzvmt.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/giguozamm.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gifmfkcqb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gomaatgop.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gwwqtbylt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gbkwobtss.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gyzmjssja.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gtqztrlfu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gqoelwydu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/goqddswxm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gkdndjxox.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gfdycassb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gnqsewjpi.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gojhealuj.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gqyilshkt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gysturhky.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnmpzcwjo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glbxiqmcz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gdpedbzbp.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/ghtayatut.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gwjxerkpb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gwccvaezy.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gptyrxxjo.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gfmybiswb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gixgppnzl.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gwgefobxd.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/glphnwdjn.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/ganmhsdlr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggpbiujdv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gotqxnasc.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqbvevqzo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/grvcwmpgc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gfbkbnict.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gjctgieiz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glnvtdnnn.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/goqqbqkgw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gcekgqkvf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxkaxilgw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gjbcihlcm.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gaqidbkes.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/ghdkkiqpe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/geulqxjsf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gijrnkqnl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcngmpkef.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/grjtiutne.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gfskytjrd.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gakzskzvw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gvgqlsqdv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gpwutnidq.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gtvliicwz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gervmufav.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gwtamrdfo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gspnskcfb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbiyzucpj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gsadxdxqw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gxvbzepmh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gqnbgoqjq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gpzaauvbj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/goxzfdays.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gvbixoqud.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gwmoolknf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gxzdtrmpf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gqkxopqqn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gtpxpefii.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gqgvvdyto.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gryntadcp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gkxpaivpx.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gecmnftkg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ghsmpcsfq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/ggdqtxefr.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gmdeaufpa.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbgwumzmm.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gygbflray.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gvuwpvfac.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gakpuyjso.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gzkrfkkzc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grrzpxljv.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gogacpykz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsyeonfnl.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gafqhqdey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gsrowmtwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gvdwlrvuq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gwffimgfw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gmbcsfvkm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gnqadiygf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gxyjrszxb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gfdbcebbc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxcjdreat.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gkbnktasc.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gqnjpsrao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gnsjybvap.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvuisgiqr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gextfvdbf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gctvuavle.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gwqujiczd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/grrufchfu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gyibjeoml.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzssxuvjs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gcxgsqkmx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gskqidokh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghbhdtcmn.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gzqirzmeh.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzzvomzkn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/guakqfqbl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gqktsychv.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/glosiipvl.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gfuiadyle.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glnmopzlo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gdxbojbtd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gercmwekt.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggndclifr.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkamlfqrm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gmdtqunev.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gpruppart.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzkwndeau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/grsdtmruc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjujkevpm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gwbckgpbq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gzueimeah.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gdqimjzdb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gsqwwdrrx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gqxghfnyk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gstixbzze.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkbsnddav.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/ggacerffh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gojwazhna.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gmeowthyl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gacoafits.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gcesdanys.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/ganbntyxm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghpbljybl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gytkmbtoi.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gletmezup.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gitdjpnmi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gxsmkhlnv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghjryshgh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/grgctiygx.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gfnsferuw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gozvopits.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/ggifoydva.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gywslfqbb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gooulfvyn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gcfyzlxhc.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gbozuyflw.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gmuusyylb.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gqnrnwutm.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gjxpccrmd.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ghfhqijpu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gkctddqxn.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gdqiyeslz.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gftipzrzz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gkcobjrum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gkssmszqh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gvxrgiqja.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gvvyyhahr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ggsyujxqq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gmwgiwyxq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gjzyigzmh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gtfegxybs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/grasulsly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gsxwwchuq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/grkaofhbz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/ggdnhtwpg.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmwuzffyl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvuwkpzmd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gmqbudbti.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggiqsfpft.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gtqrsnzax.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gentbvxnt.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvyfbweqb.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gfivskwdy.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtxwgkbwh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwbgzslpw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gjpqjibkp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkopwfthy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/geeumkixv.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gvlecsnsz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gdwhfwuat.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gkzpvqepw.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/govbkmysc.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gnnarmxor.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/geioxshhh.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gparuxlud.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gxhllvxdi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxrnccrss.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gmsathbqo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gybdevkzm.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gxnqclssx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gvluliggq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gqrsnoivz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gykmjfhaa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggcnvwyks.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfcboclt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/ghsclifju.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gicdyjset.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkdwvjzjn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/giximnezp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gyvxndiqr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gbckflwqr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gczpjpgkd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gufgozkuf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gdwyhrfhi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gatufqhph.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gmgkwackp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gyqivubex.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ggokltbfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gekuvmthy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gcvhuntqz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/goqemhari.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gbbfbdznm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gcnhazlpj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gtxjyqsgl.sHtML


<!-- 参考信息 -->