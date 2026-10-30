代发 wailian999

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggmtfzgmb.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqmtwhjca.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gcpjhuqdk.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gzchlisxf.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/glxfubolb.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpvgtcdlc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/grkywyhyj.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gdiyvjvnr.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gjuovyhlw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/grsvcizxa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwrsbtihf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gzfevyhci.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ghcfdtffr.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grjazadeo.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmnbqcjcl.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gyurnnoju.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxawlwayt.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gwqytxomc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glwjelsjs.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gwvsgbmwi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gaskxcpft.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gcpoyvacm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/giqrpflcz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gmmensufm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gxfxcalor.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ggngtbojc.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/girdjyonu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdrzjmpfj.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gizfoxskn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gfykklvul.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gnwrmgabj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gfhjpkzfb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvhhbmhpg.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/geckmgerf.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gcadqdyhx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gvwslvuft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gaybdcfas.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfhbwbvvq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gpuhfxaqi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gpkymfhkt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gkqrzhkec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gphhqyhsj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gxoifncor.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gpckcdbgd.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gjbppcfof.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gqwgrjxcs.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzzqoqjop.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gxptpgngh.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gwotyhoqw.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gtdghujyf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gcogmbcap.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/ghxsgfwyv.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgmtyou.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gmuujmttc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/glcujaaoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gcxejyfcv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gmtahifbl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gyindiszt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gremvidav.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwxmqgdbx.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/glvbjsnnz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkufnfgfd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gzqtmpixh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gqeugpqzc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gpzcueefn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/guazmmlvp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwolpbvyr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gqudmzmty.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/ghwelotpl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gmaanayjw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfjepfuvo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gizswgkfo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gpgdglycw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gdkfttzjm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnsdgvjxj.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gijouzmte.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gooyjgesm.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gwrkcbpfd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gffcmnhav.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gisrhbdvq.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/glbgkqmvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gofddvnfv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gasmlplyz.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gkfzgcgwf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gunjwdlxc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gezstutvr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gwvullyut.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gipdtkday.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gnbohzeah.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gwghczuzl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gkuupjlde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gzrfiscei.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/grveyjyoz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gwkifuzdd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gyhqhbpxw.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gjjmfzedm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gyropsiai.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gygllpbrl.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gcvegysgn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpfzhnxhb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbqnvtzrh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gnizzaior.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/grdhszszk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gfltzyopv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gzupzhahf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/glwwpmlvz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gkzxphcgj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gywnzzxvj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gflihwynt.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gybzwssaf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gtjzsvteq.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gmzajnkzy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gigchvmuz.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gjsbrqsym.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gqmtzvnoq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/ghqqzwnpn.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gdaqdvqtu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gyuidygmu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gfzrqdfnk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gswvqorjs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gnjvgozbo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/grdhyilaq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gfyefutbm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gmgempqce.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/ghqhklvci.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gpdqnxixe.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gshkwhrfj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gubfkzuos.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gkdbjgkvp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdwnfidmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gsadibeys.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/glosnbjfo.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gthuewjyc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gzscbibzg.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gxcjxluja.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/ghefxmuoe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geqeaoxnq.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkpsjnskj.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkevetxzu.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gwwdxwsex.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmagkwhvx.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gpsjabghp.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvznfkmdn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/glbpraycp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzckkijav.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gsrhkuizc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gigqgdhom.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/garrmmbfj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gyxpugftd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gsotvjqlw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gonyfsred.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gsmrrgsdm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gstiyhtga.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/giffhqgvr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gkjkpyqsk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gjwboqxxq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gdpohillb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gwacfvvvo.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmnicprxz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gebeomttf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gopznbdik.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/guvycqqlc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gqkvrwzqs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gvysvjwos.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gsftwsztk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkdyowhwj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gocqjsdvk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gmwjsjuoo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gfwyyttjm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gctfebwnn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gilckhzxh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gttklhzig.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gcdlpvsec.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gscljkwre.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gyimbvmtz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gofebkgvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gqtomloze.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gaprdouvu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gksyogweh.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gloeluzra.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gqxlkqall.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/ggyhgnzpy.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gpngwbhap.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gqnpnhfys.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gfiwizyam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gbwyzjnuw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gpfjjqulh.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbnewyvix.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtroqgcge.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gsncogxhg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfocqdzbh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grawmlnur.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gxrvbgvxb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gxlgwjchx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gdddcexqr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gwcuxmfrx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/glenrqezt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gpfjicaep.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gwsvcxgrv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guexatwls.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gprlwnluz.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gawfmxewl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gzarwkcqo.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyauyezte.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gpgdjqthy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/geyvkxqqv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gaxiejjsd.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gbrmvpkxj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/ghquyzrvn.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gcmwlanlm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/glizeclyl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbjzfskqw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gcwhcjixr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggmuodhbr.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gnlhiopdk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/ggaghukxa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gmluusgxc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gppzajlaf.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gwwtkwdww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gvgyldfrj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gpittaesc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gwuiepxqw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gdkibbcbc.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gmwmtkdii.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gykbklihu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gvqpddwnv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gybkabepz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gbiwgvcuo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/grqsymaot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gorrcncnf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmtrlvusp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/grgbxsrhs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gvxdzgkch.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gtfkcbulw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ghwzbzsiq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gpawaxhuc.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gdevxseko.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/glribgpwi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gblknaole.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxeopjjxx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghyrjgjub.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxlqrpecl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gtqyvjwbj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwobpmmwq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfqrrbovt.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gkuxtbxxw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gqttwolyp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkrxonudm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gpnsrlbin.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxvfyqtjx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gscdygypv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/ghwxkjwps.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/giufdounf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gqrtgouch.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gcrsuiwqp.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/grgazhmkx.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gbcpazbsp.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gddppowmc.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gjmcwqodb.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gxnmrjybv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gqhboeozc.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/grltntjrj.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gciebyaat.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gnzuamhgj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnnuwkmfu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghzrbzhtl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzafuekqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/geenyasgb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmaojjkb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gbqpggxwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gbozgevpl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjblpiklr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gteakmeda.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gahtbdxdh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gbwkjrkfu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbibliyts.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzevzszir.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glntvhhyp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ghbcadkxq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gjbdkeryl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gvffaxmlb.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gtanutppo.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gmjpmqhhu.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gzjwtqyie.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gereppqon.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfmpmbklz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/guewtqwma.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gssyoygbn.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gwvqtsxua.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gianhwgva.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/grjxlgudt.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ghulranyg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/grcykarfu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gsvyrqfix.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gqskgrnwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gsokqjzsw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gsiqclxbr.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gubnwouje.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gebovnphd.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gsfqfxcku.sHtML


<!-- 参考信息 -->