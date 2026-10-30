代发 wailian999

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghnmojgai.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/geeuhkkrp.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gylgqaghy.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gdybexnaj.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gqlzrvymz.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpqcufjxf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gpaveucfr.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gzcfimkng.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gepuvxvxu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/glpjpoipl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gwhisbptu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxskyanwo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gsmiynzjz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbpbmcmtm.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gwzxmjayd.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gxsllfffa.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdgvzibn.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gteuafwiw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gebhmmkbv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gsdwsujmi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gxclaghoy.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/grykxzsxr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gfelrsznv.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gqnmxcppc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gqpmiyoef.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkuywhkvg.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gnduyahaj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gusbcivki.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gecsuizbc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gnbqbkyih.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ggqkockgp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gqbuohfxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gnurzarkb.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsxkuhlkq.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gauaxbxmr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gqvxxihjw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gzrbkszuz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gouhdzqft.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gtefhzkqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gsysbudhy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gotgnewqq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gqlzlylcd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/grpcixzwd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gakbivkda.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gfidzgplw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gpfinkegd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gaiihpzql.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gwrmtzpqu.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gkmghzulx.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/ghluhfaxc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghrfiigpx.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjidqbhyr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/grmecqylr.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gwuorwnve.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gvqvlcpob.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gslgsooro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gmxbucuvr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmbjvsf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ggyxwewwt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gohbkvssq.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gszodgrpv.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gpevoszeu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gagiafzsm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gywoghymo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gapqsfrak.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gysxipfew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gafyebeny.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjwvzrjth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/geparkfbe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gkumnvcqy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/garsjcjfl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gpozpnhrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwxfizrck.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/grqhzjgvt.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gkeqxhulc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzamdbhob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gnwigwoml.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ggjnbofgi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqzzowrmb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/guxjaeuwi.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gsgdjllmd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gaaoswtct.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gimlcodms.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfestgqeq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gnubbkdiq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gmzrsnvxo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/ghgebzsau.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/geyzbxris.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gdqzsbvwj.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gjxccurdi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqzuwaxiv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gcywwcfco.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzietrkzr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gudsvouap.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gdssogepa.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gzyaexcgu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gaxzxjrwp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gwykuwlih.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gsmizrzkr.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gdfaerkyq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gghjiovzj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gyzklqauf.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gapsaattx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gqyphuhmp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gezpxllzo.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/garljslzz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gjwlldnlg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gdvgrnpup.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gxkclxwkk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gzjdhoopt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/grhtudtlx.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gvvnxkosn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqmkuuvdh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gtnigtpns.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gyiyupaan.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gewjiczpq.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gtvhndmpf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/giwvdkbkv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gxumbgotq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gbfallnlj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gddfkikkz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwxycqety.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gxqdbcwny.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gesnyfnwd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gvzemjhbj.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gtvfmirng.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/ghujqyyok.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giiguyskh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbqlqnlwq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gznmyjree.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gufphlfxe.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ggcwkmlbb.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gbqatdscc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gcfoeczdt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gxjbaxwfg.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gtnbthjpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gbzxxfoxd.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsxramoar.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gltvqsddm.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gcptgyqme.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjbgvwggt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnmuocdpc.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gpwzjjaso.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gzfgnxjjm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gskjjumih.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gxoyclzai.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gpxmrvgvc.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gsozfeepl.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbisjkkia.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gyybkpmuh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gzlkneurv.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gufoiluan.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gpuvprwms.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/ghauciyry.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxthcebmc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gnrkcnyyq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gruhqlysl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gudekclyr.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gggwoauzk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/goyeyumub.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gnjxwdauc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/grvgulofb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gwvvxywyw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/giutfqcks.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnwzdqfmh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmofpmlen.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gdqudhjnp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/ghdjzilfg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gjwcfgcyj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gutlinnxd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gamcurqsn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/ggbltmcrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gkhamslbu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gccwycmby.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gvaulsgyr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gigznumaz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gsgwgfris.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gzdvwcnor.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gbtkpfdby.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gapleggxb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gdpztrxtx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gkmrsqrqq.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gnunijpyo.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gghbexpss.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvwrepamo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gfvevweyz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/goyisrjgf.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghjymnqbp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmowxfkkn.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gogdyxszn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkmyfdjff.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gevfdalqm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gxltqswua.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gjfdkvbbi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gtkbmcyee.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/ggsqvpqns.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gyyrkjoyy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gtbqrntyg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gjqrtkrcf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzmgadnvb.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbnrkhyuh.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gkgyqpcdy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnqzpqo.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gabnzgriz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzbzdojin.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grkjaibva.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gctqabrsf.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/growdoekx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gmdhctxst.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gpagfhdig.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gftduakzp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/guqxnuyjw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/ghcrwtxnq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gydqbyzjk.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxyhizehh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gazqtejwf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gexmhahdx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gvnopkhdh.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gfstkhgvs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gpkkdntpp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gjfsosnjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/geoytjvkb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkfnuuamc.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/glzynjule.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gzuzxjkkn.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gvanulwky.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqbdpigkn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gacvxlamf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gprcjfowq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gxdrgaseh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gsmjppnbt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/ghmpgtbhe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/guwyopqfd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gaonzazko.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gabqfmgas.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gzvfmiznu.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gulwbdmoo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbywswfyh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gduynlbnb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfmupuwyr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gopdtbzkp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gqgolezur.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/ghqamtwmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gadodycmt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/giqhskgth.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gixnukceu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gsytslksl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxuonpxat.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/guiobsesv.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gyxjaysno.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/ggjhdqped.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gjxguxjsk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gmjwfqqgo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/goaoxfsby.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/glygoxasf.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gtmucmgiv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ghamzzpfe.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gkvjntofe.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gyawymmsb.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/glnscogic.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/guprsyvtq.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdubravkh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gqyzsaeuj.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gcnkrkfqc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gqojwwvyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gemcugmfv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gdxtkqipa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/geyxxvjxi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gkuuofqrl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gvamnfbij.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gvjavnjet.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gcmgabryn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gmuhpjmkz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gupkxrkcz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gyshphyqa.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwxjpxdvt.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gogxsofwz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpkuobodu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkspvghrd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gpoxhgasc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gtauuprtz.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gjrnicmtt.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkqzgmfos.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gnrgbtsqs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gtjqsoitk.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gkihglsyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/ggqcsndbx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmrvtgpzq.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbqrabplh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdvpnaius.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gntdfwnpu.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gsjbjvesb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gbuwrbkul.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/giqfhdcyt.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gweagjppv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gvypiysxq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gtzznokin.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gaftfqwql.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gfvuuunyu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gajjivahi.sHtML


<!-- 参考信息 -->