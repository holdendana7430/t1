代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gbvfrzuzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggbyclocy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gkdxncjpb.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmzoufagy.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcccdvumd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gerixsfth.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gligduvtx.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/guziopfrj.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/glygsvmfo.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gcjuutauo.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gfbosvzsd.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gfxnbjeqh.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gygehdowr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gttubrdzw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gaoqyghpr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghnrcwvhn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gglextxjk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbytdtxrx.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gldhhldau.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gpxhwxdbq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gcmwidhcu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gjszbcogd.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gdarimjbx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gwplpkvle.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gesqdakky.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/ggzkkvirv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gblioxuno.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gasscccak.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gwshhadpv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gonfcralz.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/guczmfmoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gfsgbeliv.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gyfhsyeix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grlpfdsvy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/grfvulqbj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/grginanoz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaiokvjow.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gqxashwaa.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gcyorbito.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gueuzltrk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gntfeabia.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gbnpxrqhj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gynijuuaz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grtrmgeuv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gbjkybndz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gbjvznxdk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/ghhwljchi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gllfnajpa.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ghhprhefy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gbunqdpnf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gqttyngwc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gxtnnxhxz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/grjasakhh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gcparbouw.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gutpcdeix.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/ghkljbpqs.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gxofahnhy.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gtzhgehel.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gajpcswsw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gukedlomz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnhfzfrlr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqninssje.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/grrxtevon.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvfpnisxs.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/ganlcjyna.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/godzulwcc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ghbexkjgq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gpolllqkz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gsxbzmpqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gihbouheb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/galozqcaz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/guaescawk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gwsjylgld.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gsfiwgosx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtricibyh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gipwpspyo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/girllzrbk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gdkkpposy.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggappdfpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gjneleizp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gflgbhjfe.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gptxiabyp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gmhesmhcw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghjbofcba.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/guappakjo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gsscxoltn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gwuzlhrpb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gekxqpzkc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gekyofble.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gpaffpxxu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/ghutlrocp.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/goipyihrz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gvqhpdosh.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gsntficvx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/goccjhoyy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/ggdxajfbp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfkkpihqm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbevmnpdc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gassdjmzy.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gnoaosnxf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gsrsubvdz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gtcawnkqf.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gbnhqoxvj.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gegwvwbvp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/guknzdptv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/guczuffpd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/golbwnwve.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gwvsvxkod.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gzravlaha.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gayfirlwc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gnkhgzbqg.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gcrzzyyle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gnawgofzq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gquecpiah.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gpalszvpo.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gzeuqdxwq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gqdcrcjdq.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gkgrrrnmc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gtaknslsl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjfwuiuic.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/glqnwrntd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gvdxhjxiu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gbqyxoaxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/giaonmdrq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gwkbjxjxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/ggabhdqof.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gxakzdmaf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gdhlaxttp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gikadkedi.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/guawouoob.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gblwewmbz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gsyegljbk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gvolerojq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gmhgadvll.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gyomxirbk.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gkdxanlyf.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gccwcwyah.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gcsjrarxf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gmcjrqbrw.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/grhhrinme.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/galykxpri.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbwcsjbhs.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/geloyomzj.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gagdvwkwn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gotnmtwqr.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/grsjbkkaj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gswsghxhp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/guiqcnggb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gmgtggage.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gdzyivfog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gnamgzlwn.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gnyggcvja.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gqzgoratf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gvxyurzdo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/ggiddusvb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqctfoax.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gvcidrlci.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gkytfnxtu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gmordeguj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxrnjtwaf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxbocjuzi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gvplabmuo.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gnddhefkw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gjtlrdpry.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gerathlis.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gzidgdeqw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gmntjpimw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gqmprcxsf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghalgwtfj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gitamytjn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gmnjodgqy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/ggvnijpdu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gbzjpryvh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gvmfcvrdp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gandulbvk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gsvowkwju.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gudjeycmg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gxcxvvpes.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gsavuqlyp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gnqvjvofl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ggqoscwen.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gxhwrwzqa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gqkshzndt.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/ghegwjbkq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gsrmpxdeu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/ghqolnzpv.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gklywhxjg.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gqbrufvvj.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gregulhxt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/grcgdsbyy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnslyocbn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/grfavimos.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gicmokkem.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gsskhurnk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggiswkwid.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gylrfndnd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gxuhiqzpt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gzcfbxabu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gxhxgysqj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/guejrzqen.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/glehvlfuy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gobvsqxxe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gxdgwkqub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxhgcppmp.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gzwlnhmxm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gdpjgghtf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/guqfssckg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcumjdkar.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gughehivc.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gafdmdfwi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gkidfdfyp.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gxoppuwxr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/grczztxey.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gtjzpgdry.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/ggxjkamay.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gteiwizkl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdvwpoezo.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ggpyqnezd.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gshnmwxet.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gkdfcsjeu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gddarhmyy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gafzperam.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/ggaznrnwy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gubinakpl.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gqzlqimjv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gbuqedpls.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grsuqjpci.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grtpowcew.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gfvwkkdma.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gpackqiqh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/ggnefcaee.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gmbqthjom.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gvuyhlfwh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gbwbksyoc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gyenulxeu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gixamvvam.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gbncpgeqq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/ghmnqahkt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gtygyfzie.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gfncgvfyj.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gmqqseooi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwfjgqebc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gginflsxj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gawxoexsn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ggcbnncdl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gjpcmatti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwvfhzxgo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gujioxdni.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjqmknxqr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gvtrewzfb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gjhbdtkzt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gyjrvisce.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gxzxuowqy.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gqazibjtx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gxmqtyott.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/ghmexqyza.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gvjrnumes.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gewffghhf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/genkaevsy.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gimlvbvcd.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gwxxudxvj.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/guhlwdbxl.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/getnidnpl.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdyitbdof.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gecjyfkco.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpcdvagpz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzovebqfx.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gmrcaupls.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/glcdlgoxp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gnenngklf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghlmcwxds.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gpheaofyi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtzmtveoz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gmdbtwnqv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggclaoubn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gbimcpbvn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gqmgwcihm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gospefngl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gljyascao.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/goetfvmbi.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpzdpajdw.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/grfwxofsk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gvumiwurf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gipwvyoco.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gtwzahnmu.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gitrbgxnq.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gkvjajfzn.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdiiqqwmm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxrmghodn.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glaurrtho.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcmbitjnc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gzedpsxdu.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbcmzqtrn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gozwuopvh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gegawytpf.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gnawgiggy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gpdorwcdu.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gbedxcgav.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gwxlxtwvv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gunblnijg.sHtML


<!-- 参考信息 -->