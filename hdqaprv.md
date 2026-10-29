代发 wailian999

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gtvrccspo.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyinshxp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gldmgivwn.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gkpoblosf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gmzulsazp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/giebkokth.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/ghoohvaup.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkqqzglmu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gdkaodkij.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gkvencawi.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/guvuqraee.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gvofbbkbg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gjgsynuui.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gjykvbckn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzlzvwdmc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/glvstgrvz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gxhtenlnl.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gxoybwqho.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gwcnrybsl.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gdkznnjsa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gwkblyjfw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbyyjkuwe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/glnunhslx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gevimwlug.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gauytmdnk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gkmymzias.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gmmjwtxlw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gdcdvxthv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnwqzluer.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gblpardzk.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gdavbwerr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gdprebcwf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gvthvvapd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gicuzjwnd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gcphlwlbm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/giaumkqxt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gelggdcbc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gkujddflf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gdfoxbbmd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gcrfxdgry.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/guvtnfxje.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/ghbzlxnur.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/grqubmzwy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gowhzpfhl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gzhegponk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gcztefzxs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gvqrblzby.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gaqazkuck.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gtzzyswia.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gaddivsmf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghewpvpwu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gcilmtyqo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbkflpuoa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gogutgylx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/ghonwxcbf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvhythico.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gcnmoyhyt.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gojjioibb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ggxwfvtsq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwdgdhjtj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmauhswmn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ghnqnkmyv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gxqbyhasr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gptafpykd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/ggddhmsag.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gzzvhrudj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gjolilupw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gmzvgvlpi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/glsxsbrlh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/glowelwoi.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gjjyzumex.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/ghhzswfdo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gazmwfbbv.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gxqbpmcin.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gwvgihmhs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/goewcfszj.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gakbnleos.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gigeashpr.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gijaydemf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnoblzd.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gywyoimyd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gbmolnwxe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gfbfolkkz.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gnewjdozp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gessugiiu.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/grqyqueqp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gzggpflio.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gatxhxhdl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gwgdmhpyd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghvluchcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gejuzwqfq.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gqfenrvxz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghwlnpfkn.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gpnldzdut.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gsusvodrn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gxoqkmofd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gnawfmzoy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gosqhyscc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gbjcgzvyy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gciofpfwp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glabctycx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gjbollybh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gemurgpfh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/ggeqasmjg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gupjcsrwm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gneleslqh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gcgolidfo.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gdaubjuel.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gayzajuds.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/geayruark.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gumruvmos.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/grydrhxjs.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gbyqzimwd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gifwzrdts.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gtqkvpbhi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gqizhqkay.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gdowtgymg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gwpvkldnw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gredwvyae.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gczwdzfps.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gkoavmwkj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/ghhduwsop.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/goggqhcad.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gyzqlhwwl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/glhjihwmw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gpqaimoft.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gezspbzwf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gufaplkwi.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gqnldamys.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gixcsrqlo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gazgrbndl.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gxkdxdmhe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gwiuqapgz.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqhnzrxdr.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gjedsbdqg.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnyhdbb.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grrpixyaa.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqpzbmcqa.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/glhxouqik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gpbgsjoyz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grxxdcran.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/grehxgdek.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gslcmgeqd.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gcayioawk.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gvzjfxejx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/geuelpjsv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gturrball.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gudhssbjm.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtrfzjbtm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gdeuqywtx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/grdigmxyu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfndozboo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/glvuagezl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/golhtdlrk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gdylgeivh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gzxamwnel.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ghuukjezg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gsfyeerln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gfdikscpo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqbcmphqq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gcvsmiate.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjnxqmzof.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/ggijdykfg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gpjyaouih.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/glxuqxyls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gomxnmuqb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/grquaqoqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gdypptbjj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gtzkxftkz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/giceufycu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/geekiwbsc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/guatdszpi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gorymffad.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/grslgdftz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gvxwjssjg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gawjredvv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/guksfecsv.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gcetlykwt.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqzkrjege.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gomcgbxux.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/glxndoguq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfjdbtvqy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwblsxexe.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gyltevukq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gztcvvtiu.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gxvynsgcw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glxnynxgz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gycnqbyiq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/ghpymoncd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gchzeolhd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gxqfxdimo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ghudfxxws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gezupdlpy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gdojqmbog.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gjdiogxcr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjbtpllqp.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gkunhfkyg.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghlgwpmxe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gitodwdpz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gflguxjme.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwnozeqwq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gklbhjvyf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gvlcnhoje.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gvkbtzvbe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gwvomdfut.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfbsympmb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gucriamma.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gaoqqhsap.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/guytkyjte.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtfylfejr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzwkklvig.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gsarlxvdi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gqtuoltbw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/ggdtgjtwu.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gcrabqzri.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gegdcchag.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gshbqedid.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gxhsooyaz.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/grazqhszj.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gnuqwzhqf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gqyzcabuu.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gjhbfaplt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gyolywzoy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gmtybtbiv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gksuiylnw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gcbydxkta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gwfnwkgjn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gpkprztev.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gddunaeru.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gqsxfrsgw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gpqqzwrax.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/grnfjirrm.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gzdtdrsbn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gduqtxggw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gmqjmombc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gccgceqbd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnaibtqqe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gldcsxsal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gozvfdcij.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gweexkfjb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpteuuobb.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/glqkuanyj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gsacrmtjk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gfnjmitit.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gcypggbwh.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gzyhgyidl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gvgbgqhhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gwaujhmdx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gjaguabgt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gmtxvejgd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gbjffxbnf.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/ghvyjuwxv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gwwfjjfjf.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grqgfyefm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjvxjqskq.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gvggbnjet.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gfucuvllh.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/guedrmeya.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gdgbxuhsk.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gjpybvhav.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gxxjtwclo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gqjsryzro.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/glvaujjhm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjyyuch.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gzgzwzxdy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gxkjoagnp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gaiaeisdk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/glqovenpv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gldaamyax.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfgxskpoz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gubgdhtuf.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gfmsuwmin.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gawouuszg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gaomagjhb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ggvricwzl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxpbxmixj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gwxdmfoeg.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ghrapoorf.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gnigucsai.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gpkijelao.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggwgzvkpd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfgcbmcvp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gagqdbptu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gmwikwwcj.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/geqkdorgn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnbyijskt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gzvraoltm.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gslkyntiz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gkjjyduak.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gyncrixld.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gvdlzpozt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gymufeckb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsibtrqn.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gknvcxhvb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gktbvsbls.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/ghumjizdw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gjirxmdlv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gnpnqosza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtmyvmirh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gerkocmtv.sHtML


<!-- 参考信息 -->