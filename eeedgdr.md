代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gilzqejke.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnkbmzvkj.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gfumbujgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/givnzfitl.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gavbhgggr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/ghhhvymoy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gupqdaypn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gxkdjtbwc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcmwbndbj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gurralrif.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gqbblblsi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/goeaauzci.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrojcfuk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/grzgyexeh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gwtyvgtif.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gxtevqqhs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gbbgqakol.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gxlityrna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gknfpxmuz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/ggipchlhq.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/guzrvqckf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gsnssoxyi.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/guvlgxiuq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gduednfrz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/glirsixvf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gvjptsheb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gtmztxuoj.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gwtqrgbya.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gtluahjxz.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/giihglgxp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gqlmzzlxs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gjehghitf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/geeanitzy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gkdjsxgel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/govdtwogm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkakjogrw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gixokksbf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gllntvuwv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gsaflwfwl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/guihjgenz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gwkgjjurc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gwwrxuxfy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gzllwhbkh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gvdctgrur.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gcjdhlrrs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gtzaioweo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glsofzeia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gorgvgiyg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/ggmjxakrb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gpoggadvk.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkxqxnxyz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ghdqyntze.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gkksjztvm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gsxhcqgru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gpawxlsif.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmngljswj.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfxqahuho.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/ghpastxph.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gcfagnufb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ggaqxojda.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/geebgsyzy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gsyakclwm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gmnafgfdp.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gepmrycwy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnkufiyyu.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gncpzhgpg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwadwnfpo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gstfemxqx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/goitrhbyo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gptkpjrfm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gskfimkkr.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/ggjccbtbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gqvbefgoh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gewqqpupb.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gkgwhdgcv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsmfdjahp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvjaylelw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gnmklnhbb.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gtgaaabbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gbledthpa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ghqxjwjgx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/guocjqyjj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gihukldlr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gluosfoax.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gkjoxhfqs.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/goamkwacv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gcrjysbhk.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gjybnladr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmjbfpljg.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gdiqsqmts.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gggzwxvhn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfjegfwts.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/glrcqnnza.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gjalpqzrl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gojjqwsgm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gcusnvuun.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqohzblbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gmlzohevi.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/guoqopjyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gvnlaacrg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gsbkqafsw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gocnrfbee.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkvcxsrgr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gvvzdtdcg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gbfiyekva.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gvdtaiaet.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gdcuarujm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/grqhuaaxi.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gyitcpmab.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gcxrdjkqw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gnwakgjot.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gcpcrvspc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdvjtnask.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gapmrobwl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggpdppqpl.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gcjfdcvao.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glzhxxavu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gouylajeh.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gtghnzoku.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/goutkpgnl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gfjpztvlm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gmbzrozrg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/guvaiahtc.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gmopneqgz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gndfnbeor.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/glkxydnpl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gmafkxhrd.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqqsmhlya.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gehietcpe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gharthicu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/goxonckql.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gwkqtzmox.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmebeykhl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gqvwgnupw.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghfoywiss.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gpjbiwwfo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gtwarhdrv.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gbeyxhtay.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gqratphoc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gectztnml.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gyhjqctsy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxemaixb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvhzcgxpr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gfdeaxiks.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gpxyfsqej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gausldcjq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gsbtqkeqn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/grcgzuuwb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gngzdpbpb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/guilfbxev.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gbcxcvell.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gasbaetxl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gwunqjihk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/ggytmcxfi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gqzhsrzno.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gpttpagwx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/glwgztwfb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gpcorjxqk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gsmlojefw.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gahozmeic.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gnnzobvni.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpfmyctzn.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/goslhkkfv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdknjayrr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyurrsyww.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gdviuzldn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzenfibhi.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gndnxzotj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gnjuzzcjq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gxlnnxewg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gabrfpewi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grucnhmkd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gghtdurvr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/glzzvsbja.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/giweeyimf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmrgqjueh.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gmxyrcyus.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/godnpnrvv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gzuuwzbve.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gifgxfejd.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/glcdedbyl.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/grxcvgggk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gsifukzij.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gqlzgpaeg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gtyxgqdau.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gkmtgbowe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gvyrtkiyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggmetvkod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gzcwkutip.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkpqyizje.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/geihnshja.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/grbyawbcl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gbcgzyqvn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gmkfqkguh.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gfqdgqqxe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gnrqtbkvq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gyvxafirp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gaxksmlum.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gyfiyhkfb.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gxrphemwa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gvswhomxw.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/ghpyihasv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggtuyugwr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gdncxvmst.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrjofje.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gnnmyxfyt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gtduvkevo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gqwnfmpps.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/guuqaujjg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gvsjzroil.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gitmkflqf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/goihoyyxw.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/grtvniymc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfpazfhik.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gbrkhlweo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmgtvaakc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gasoctpzj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjlsfcgnf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gvtlpsawv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkrcwdpcy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjsvltooj.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gvucqpflk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gbnqdsblq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gloxhsyyc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gnhkffaef.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gjkroeznp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gkhlkpgay.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gmrfwwaum.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gjxkhdjik.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gsmrpvupj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gwrkubjtw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gomdybnnc.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gmsicclnh.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gpbugfpbp.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gryhbmfez.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gebpolygc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gjboomnsq.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gfkrjvfbk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/goakezkex.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gszzgxqiu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gayecusfi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gvlafquaa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gkztloxuz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gwdyczbko.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/guvqdvkvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gykivrvgu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gctyhcbeu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gphtaooay.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gsbaepegz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gsvjgoobe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gesbvjsib.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/giedeefrg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gyezgepuw.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsjpciuit.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gwqmqwant.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjxidevwt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gynguwhpc.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gohfcdmba.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gyufomcin.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gqheeqhrd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/giwbhdplb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gneycsgrb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gkrkajyec.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gxrcqtmvi.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gsjlxtbrg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gajwdjxcd.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gryoewrfl.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gaazkohud.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gvuwuajez.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gahvbqcpl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gvtzjhygc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gqdwzzcfp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gmqfluqni.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gexmfledh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gjzjhyzgi.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/glgoyybkl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gmygyfqby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gutsuyjvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ggccrwnpg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdqiwwxil.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxdkyhfym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gsizllqib.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gbyrrplne.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghexggjcr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gxcukvphw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/ghibjumsc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gaszpilkw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gdmhbclrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gzppfukof.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtcqspzzc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gffmrlcly.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gccbpeliu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gpjiienvk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gkuntxvuh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/ghlvfytnq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbjmizqao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/ggodsnelt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/guiwjcuxl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/glouzkefh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gkhhhcndz.sHtML


<!-- 参考信息 -->