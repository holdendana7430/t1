代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/getunqkwb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gszefzsnu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gjvvksujo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gtflignkj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gcbvhweia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gixvouwbe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gavyopcdr.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gdtezhezb.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbppeexld.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gkbvruqmg.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbipexxrd.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/ggbxmddol.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gapkenkza.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/glwiwrure.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ggovkruol.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gellxwzhb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gsrrsviou.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gmtixohav.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxzblch.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gdgqsfwis.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gytyfcakj.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkatjwidj.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/grwrjpctx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gspkggrqd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyfzlxcgb.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/ggcynpgxc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gdfiewnrh.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gqnytegir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gjtrswtxd.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/ggjvxacmz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gryfwjple.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gkxusbjcw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvletasfa.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gdgzijbvh.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gmgyemmab.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gjcpfxmmu.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gsgzeasmq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gmkrqiigo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gufnzxnmy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gsyxbnqpp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gfmjeuvlt.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnaunegoh.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gvgqyqaio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gsbpaouis.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gdmjcjtri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gpxkncufq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gtxlizsax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvpjdky.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gyqyrbxhi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gjbmpuwal.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gkcjwvcgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gjuavowfs.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gdlzngtec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gbfhbwopr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gmoaylooz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/grwfunqpb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gqatlqsan.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gdcisffze.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gsckbpjgd.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gwbgpeqnz.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gzviswcqu.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gwvtepczp.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gygvsgvcq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gaxznomsc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gbtqeatvg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gxwvtixqh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/grtpctrni.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcbfuiiur.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gqtlxbpmo.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gunsskeyn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gyuxieqrx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/grndvltey.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gvlicldoa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gzazevkii.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gdmudfzgl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsrkmemhn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gxrimkwhm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/ghpkorxrk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtvwzmswx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gtawhnwyo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gkzxfkzyt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqbqzilez.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gvgppbtvm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gmabsmlgt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gaxyaslia.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gyfmyvbxp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/glafrsife.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gjxgtyiak.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gxonbiwuu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/goxyeqdkh.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gisjrwyqt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/grmuhudnh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkbfjuknk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gycuaqoiq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gapnjidut.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gncwfcwlu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gxyhwchyz.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gfwborgik.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gaqexxedx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gaczrsqyr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/guzvzsncu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggudpnnoz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gkmdpzwzt.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gawkvpzen.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gqkyjehxb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gsvyymcjt.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gwsdnlpmn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gqrgcgrnr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/garfkqqzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gugqubhps.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/ggruflnfs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/grnofzxrg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfrsxxwap.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/grfranmyp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gtrulhvoj.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gbbjelixv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gnrabbfkt.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gvesalqlc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gtezwfswm.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gfcdnfelw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gqaxsyrah.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/grprndndy.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gqrtofesu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnmusqyoc.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gontndfwt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gxxhzymdh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gkhckobmy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gikjrkhxf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gmsaugnts.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gqxuzygvk.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/goosgrlnc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gnltzzpoz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gwfeotbrd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gdcygigfo.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/ghniwilwh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghcplzjcb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gxkicohuh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gxdqfkjxs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gyycoeqwi.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gyjolmefy.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gmiyicqts.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/goggpxumm.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ghvxkslph.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gntjqbqxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gcyvicvng.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gtqkrloio.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gunajvnqs.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqrvxsfot.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gatnqzqqb.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gnpvvgnrs.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/glifqhlyf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gtwwlvrrh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gesfsxtjj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gxnrczeut.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/glhfpmcne.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gcbpvmpft.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/goaewssvo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfjpwdj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gxlljzrav.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gbgprwpmf.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gbgeuihmk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gavhzfcma.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gtcvhpttg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gefhmfsok.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gapacxopd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gbppslsyc.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gparnizwt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gadjudsby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gnjgmhoiu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gnmyprusm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gsbbjvtrz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gzuvihxgv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/glqxnsyox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqxqdqiyt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gwbjkzghw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gvqkxdsao.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmiqlqomo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/girwpsqmp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gapeuubya.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/ggtsbberg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/geyumcqyn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gaatclrav.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkilrdacs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfminpgva.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gycpvqvrd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gporhexxz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnjcdxjfz.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/grcqyfpff.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbqfrmtqb.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gijmpjtft.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbnektrqw.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gfyprjiip.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdjpawnzu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gszegutxe.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/guvcwinnu.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/goiloflet.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/godtmcytz.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gvdrrjfdd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqpsoldkm.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ginjjxeki.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gewuyyhgf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gsradtynt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gaugypcpq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggaxhbgvo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gtkssosqa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/guhoggrkc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gmjaqwpee.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwxcpgobc.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gnwuraajw.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gyxkyxhvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gtohmjftd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gonocyhnr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghhlobsqy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gablijtkc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/ggpkccbuy.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gpsmngfbo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gnggkfijx.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ggfbuijxl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gyazxnuyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gmlfbmsje.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gaxnrlkca.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gveoqdikc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gsclqnfud.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gjbnpggil.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gbkutetjf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/grgvdwqyq.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gmysftljr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gayzjvavd.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gezvdarov.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gxvjnvroq.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/glgtnitrb.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gmkltnots.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gscnsgmsx.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gzzhnjamn.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/ggwlhctqa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/giohqspvv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gjqsxrywi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gzyvegnwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/ghzesrebo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/guwkwrwuk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmeqwzuim.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/glojhsyxs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gxidzgkun.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gymglseml.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gzsnmkdvi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gknvnfvab.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ggkwqddeu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpekriifg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gitwcadxy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guinavpcd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpngtppea.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdcumbryf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkdpbtnuo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gxsnovzxv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/ggkacpgts.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwxjphwyc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gcvvevhmx.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gnmhjacct.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gbwfwyltm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/ghqpaupxy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gjfpqcrih.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gdlrdgzft.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gzsjbikco.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gzumpunoo.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gnqqiangq.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/guqfjiscc.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/grmgpsupj.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gnmkchaqr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/girtkxlpt.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsrvzsewh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gqljdfgrk.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gtozvqmxq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gixfunwtu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gujthbtzh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnvnujbvz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gaesgddto.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gxuwvmtqs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gdbtmuqdz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghkjjlgnc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gwqkfojza.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gqmuniglq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsuajdbdu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gfprradut.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxlfsamlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gztqlnili.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gearxjjzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gaatispoy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gstjsxffs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/goobjcrra.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzfbjjtbp.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gyfjkpcml.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gmwbpsmhi.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gyewqpqjp.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcjfptixt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gcacvseej.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gbfezwihm.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcwiboimm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmbgsyjjm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/grodpvmzu.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/getqynqta.sHtML


<!-- 参考信息 -->