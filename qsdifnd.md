代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gxvxnwmkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/grdhrqmoe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmyopcyqr.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gvurkbqvk.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/grxwhphni.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfobhnjtn.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gwxdnitvd.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ggixlkdog.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gogctmpnm.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkdwrlqnw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gkxnrlecv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gygcwrnyi.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gymsgsqqy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gogfudltd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gminohgrd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvgonddzo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/giwekojue.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdzddvljz.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/groqqtbhr.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gaeyewqgl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gtcgyzyur.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gbafnobya.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnpvsimxk.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gynogvqmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gafzizpjx.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/glefaplis.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzrdhxtpv.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gfyydyaek.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gtduhrtet.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gyhsntuna.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/ghisdefur.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gtmnvvvrg.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gmlyqcjxc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gmvyclozd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gtnqxuefl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/ggewbfxet.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gekuyubhd.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gyjxhjolf.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gxiawlwze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gcsufsxlm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/ggxdoavjh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdvvqrhzf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gsnofxspi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/ginhqfbur.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gohtfmqgt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gzqbxedlu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gdxikncfn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gmrutvccu.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gdasnzzfu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/ggmjcfauf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gojdzbyrj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/godtrhboy.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/glaosdowx.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gpwblncnt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ginatnnsk.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gqultprln.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gsvlxnutq.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gveraiuyc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gcyaputuz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gflhnmluf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gigciainx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gpwuderei.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gigfrcday.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqfzyxpat.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqthpikbu.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/giasamywz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gyjrynvqs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gmctkannd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gjcxwminb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbieqques.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gmdjieehl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gjphzaqmx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gywadvqpv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gqhcutfly.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcjkbmxtq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gvtafoqrd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gvsabbkzc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gfiqztflm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gdgqredir.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gqnprdbgo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gheslnhoj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/grdzzsumf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxwqxgsqs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxtkgncwq.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gyneprdux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/glochssur.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/grmumlykh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gvzxxaiwe.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gyiseqwsu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gwtmfboxw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gbffscvlt.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/goqozysud.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gamrcsatv.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gqhjbqyvs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtbydftek.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gwzxtrfoh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmyuezngb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggtodfklr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/glnnuilhh.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gupnbzneh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gysmvisvm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gveqbbzyc.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gvebcczcq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjucxengs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gemfbdbfn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/giefwmtiv.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/ghnytslyt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gfyemvegg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpawecymz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gafevtvhn.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gqjeewrxv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gewuxgtfc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gzkezfpdg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gevllcfnx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gzxdpjpml.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gzkmhugez.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gcznmrjzz.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gthpkzmeh.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/grfbmxomq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/ghjmbbond.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gmeehchki.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gfcvgbxre.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gpigykeit.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gngrmhrjt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gshqsvhox.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gizbxpuql.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gffkaeqpx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gjqfipayr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/glqidlunv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gomneghkr.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gethasgex.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gekiyojer.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gfrcvcbxm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gdvrtpjym.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gjkycykzq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/ghremixkf.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gmsvnuccg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gvtzhyirs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gpcjukmuk.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gysslrfpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gagcacfad.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gbjhlmgox.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gdgmtezko.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gdcjaqoqq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwufrgqzs.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/ghylzuaya.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gyruarmto.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gmmkybtpc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gtmrlrhaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gsltvnwsa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcsjdexlr.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnagvhcth.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gwanxfwwz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gsajaypxx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gdwtclrun.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gzitglauf.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gudqldzrg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzjodyyla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcbfwbtjg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggkgrnrxm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gcnlsdpap.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gaxihdkqc.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/ghxnfsflu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/ggrrdrdaf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gqpqvuidf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gxjqhcdfm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/ggelwsxem.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gdumzcnhg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gtxcbtgjw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gcbvccviw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gwazeccwa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gbdltulrj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gluvvtajh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gffrlzdoa.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gsxkzvqmu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gyenysoim.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gxnoapqyc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/giqpbymva.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gibpuwhov.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/geeexiqaa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gilqjqmrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/glqymoxaa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gpcindmly.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gbaqfahze.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glscoyhgm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gyzinopgf.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gdjrkqupp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvfkhbxwv.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gwlmvpdjn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/grefqnvmw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gvkageknh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gemjfoadg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gspizgyvw.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gkartdgse.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzrvyustw.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gjlsoilru.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gyzqvwofj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gqxhwefvb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwdvcqpae.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvpiqocq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gmwcsspdl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gtttoaiao.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/garnbtdde.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzmwvmraw.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gyxdbfzkw.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/ghfnqdgvq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gihmrnbmj.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxfpkvksj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gwakjvumt.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gljqytxao.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqakfdscb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gsfzvknas.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gfdzmoazi.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/guhkizszr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gxlrnrfat.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grcwhgwdd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gvixwgjac.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/guhlhyvxx.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gfsiwkald.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/glrwawczz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gbtcwumte.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghvwspavk.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/ggninktlh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gejgiwvoh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gfdoipyfp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gpvbxwsyu.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/guitawjaq.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzaifyfdj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/glnzofsvf.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gyfekupho.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gxoqmttln.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gjtyftrmh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/goltndqjo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gyvnnebve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gljmvmsjj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gmuzkwrhj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gcitzvouc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gvlegliht.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gwpdyuepv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gejjpmvch.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gcjrlvwzu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcfckmnyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gvcljvqsg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gpehwgxnn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjwbmdwfl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gavynvnun.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gqafrolxi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gojsprhak.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gckwgpmgv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gujszdteb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gpgstubtp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfqxmyyhn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gnnfejtua.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gtbxxcuym.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gxjnhfxuw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gkmvtiwgb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gyqtgzpeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gbdlwwfoe.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gbkzomsxb.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ggfsmgtnc.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gctksdeuu.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmscuypuu.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvyyfgyvw.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gzdryssig.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gworkzsau.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/ghkokebxy.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gxzorhhkf.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gmtlgymml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gcboiroxl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gtgbbizbj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkjxazmjs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gznkafiks.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/glwnzeria.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/ghyghtutt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gsaagjtju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gknddztlo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/giopcmzzz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpmsztyak.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gkpacdvoe.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gykwrkota.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gidsrnxzs.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gypcdqbos.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzfcuiqif.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvvxovw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gzzampaqq.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/giftnrpgk.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gmsyyknue.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/guydvvivk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvfzqqsen.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghwbmdskl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gfuzvakfc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gvpaveard.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gzefvrzib.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gxxvjwzqh.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gjzkuukgf.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/glhmurdmk.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/godlpwvuo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gqoizapxr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ggpjrggck.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ggziakzyq.sHtML


<!-- 参考信息 -->