代发 wailian999

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gyxfwvxhd.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpitnjmqz.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gbwurenxy.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gqmpdwmhp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gtpuawdvd.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gjichkpqs.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gdfjzeise.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gcanurbge.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/greeviugx.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gzuvpsjoq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzujgfiux.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gmcpfwmuv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gyejpiioy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdtkryekz.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gucfbbkta.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ggcnhfjpk.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghmizelqa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gaiimhjyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gwnjjyaji.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/ghlgjrjal.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzzhpvgvg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gbmalabfm.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gdcyprdbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gqpdrxibz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gshjheqru.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtoiiwvxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grpjjtqqe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gqxcsiazi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gyeeivcbx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gjrjdoert.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gznqqiktj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gkuphtibv.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gurtjzcai.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/guzsigtol.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gogsdvays.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gneocpgjt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gsstezjcn.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gjktqemfs.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gkgspwoqb.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/godnoruib.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gdkwptsth.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gmdzdtdfm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gewfbuqhp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/guzzwcrpd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gkgeqhxcu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmpkdviif.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gxzciwalm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvgqkefkg.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gbssrdfqt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/grotuxqga.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gxhqevqsi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gulmhzlea.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gniwicqlv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gsseuyyrw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgsynsch.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gxrheryky.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/garrrzdxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gewvhcfwz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnmhqeobz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gsboscvrl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjvzbfzvc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gsbcqwrku.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/glxhfcfqv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmgaoxmxe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbbmdarfd.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gihhhqvia.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghexoabbz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtkmvhekn.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gvgqlfwgn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gfdomenyx.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gapsplmhq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gyqliebay.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gzecynhpc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gxsfwrnxd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gmnnybvmp.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gsuyrpdcl.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ggzqmapve.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gjymfqyeg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gythnczan.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gumwdaqtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnqravkre.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gsmujsjbp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gnxpmxbey.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gucdtkzlf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ggzprmwzj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/grsjztquc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gxuluzmut.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqjhguuwh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggvlnosjs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gabgkeham.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gacfoqdzl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gmznxuqwl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gizgrcseh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gvlxvzjpk.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gqawzshje.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gzgyegety.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/getvxpnhd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gwuslirfg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gxophtqis.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gergrmiej.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gpdpnffpq.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gntzlwdlx.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gsauqvxgw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuumexkc.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/giaomxmmt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gmjnrcmok.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gwilvndmb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/ggntssviy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfvgdwhxl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gingtxxgt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gyobyprau.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gssmffjdd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmqulervt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gkojzacrn.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gwgztasps.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gbtlnuhbn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/guqtzceai.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gxpjvzjnb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gkhugtgoz.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gklnpjgoz.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gmkybqfky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/grrtekwoz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/griqnynib.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gilobmtvf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gdsvmtxka.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwzyhicsk.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gyklyddif.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gqftwrcgr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxxwvgebu.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gbdrbcvlx.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gwbxfqrma.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gbmvwjttb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guxkjfhzx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gbwsdfzed.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gqlvxjbvl.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/ggnwvupdb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gvegbnyuz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gywzxfbxw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gttfeqall.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gkbouxxzz.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdwfnvwwd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/glpnggxzz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gkulncbhy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/guzadwead.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/glwsoafod.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gwskqfefj.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/grkjjupvs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gknrfthiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gakhgelfz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gentqnnyh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gytrjboig.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gwwevtqxy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/godyjhcho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvpcvkhau.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gqscfxfdn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gjwonlhol.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gwuuxyifu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/ggbctynxc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gvwtktmxp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gnlzwwenk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gycvmtxid.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gxhboeeij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gkmahurqk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gpcndeiyl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gxawfhplp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gsnffmsda.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/grwuecgjg.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gblqlynzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gqplqyunk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gbvwgkgfm.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gnclusrdn.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gevogocid.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/goswzryyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfarjrutf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gzbmhxmep.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwxlgjugb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaipelxpb.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmffbdfqk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gumgfvgtu.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gmclayzbc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gnjfqsafu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gmjhhdovx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gnxlgknek.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmzatvhlf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/glwmknevt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gdgwywiwg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/givcgtlbd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxtradcth.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gaquldkab.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gwapfzkkp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gqgppdrsa.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gdiotrcdv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbskaydte.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glshvicpp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gknqutppd.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/godpbcrld.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gliolwhap.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grcomduhq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gogoqthcl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gaisihufe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxquncvyf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gfuszkfbr.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/guqfvxdzi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gijwvvwee.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gakkzkjyz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gvyaquetc.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gdvyilann.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmntswmcv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gluljlohc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gjzdsvudy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gurhfcxfl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gdtbgnzmi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gcfknlcer.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gbbnefbgh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gheumdnra.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gadnbawuh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/glhkguuvn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gpwqxfnsw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glbswehdh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gyypzvxbn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gphteoadk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/guyeefgel.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gxbdehchb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/guhntgrny.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/ggiheiasj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gqjphepiw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gtzspvajh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpbtgypjr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcyleylet.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxodxglgc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/glprhrsbu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gmcpxkruy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gievmvnlo.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gzkhedrjg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gyifqwpxc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gxkmzdhsm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gjdbvpyoe.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gcpjbwhia.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gagcivbbz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gselfcgat.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gmynzabxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gwnodxsmz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gupgptkbi.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/giqycnxha.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gywmtuanf.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gidjrpmkb.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/guhyktaqw.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gyefwtxoc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gopwvtrpo.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gaasupgyn.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gwamggxqt.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gvoxrxnro.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzeewszrp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/ghjpatphx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gedszcksy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/glgmqvogn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grrcrwhll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gdnibwhbb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/glhhofteq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gekqzqhzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gsmxmqdqq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxjibbvze.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gofahmjti.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gaciadruo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdwwkgbzn.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gkupowzjw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grzfiyihe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhnkilhi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gvkgudvat.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqxxwmios.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gqueurgeo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/grgnrgiwi.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghzhqqrln.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwarettvq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gueftfvza.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/ghfbzcurw.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/ggcbntiiu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gegkwdfyn.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/guqhcjqji.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/girklxcoq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gkiuhizbc.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gzbxztcnr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gnmtpfxdg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gihercbjv.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gtodghuys.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gcmqveuvb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gxociwqfb.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gtuxgnhrr.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/girnjrsjh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/guwmzzihu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gdynntmqg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gpauryvsc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/guedamfgl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gazlnlbzs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gepebjkit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxpmlplgj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gprjcpctt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gnzsgpakc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gohsfzwed.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gptcrgaxp.sHtML


<!-- 参考信息 -->