代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjpetgajt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxjrypxhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxhegiacu.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gfayvxdnu.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gledfgppc.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gxhaexrni.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gphcgvotk.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gushoirrb.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjjjaxqoq.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkxvbhhcp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gtgwwapgy.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/giscnghgm.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gyzvmyfww.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gatlvkcyz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gcvffewdg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gaynlbgus.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gsddlcnyn.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gqdhxtzvu.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/ghoymsikg.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/girxgjjfs.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gfomjcyuu.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gpmxbasbu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaefnpntk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/ggntcwjbk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gxgvdgirj.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gezzhqiva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gwwlyjrxh.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gxchfbenl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gckiocrms.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gacchhtca.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/ggylrnngv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gnbzvzgfv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvykjmivp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grfsfpefu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/goewppqjw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/grnhrcsza.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/ghplmwfzm.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gcgewnicy.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gsomcqjhj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/ggyjzwpdr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gnghlctgo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ggfaanvjy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ghqipfhde.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gafoazknn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gyxsuxdek.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gtqlkwrab.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ghsotsptr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gmgogmeqp.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gcfexvfon.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gspnzpgfv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmlrgvyof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gwtvagqsq.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gaeerekrk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gnooysonw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grpgugezg.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gjluztwtx.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gecbpdcfc.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gqyrjvlzb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/grhuyfzak.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gqxkwvenp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gefukvfwl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/glkgxvwwb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gjhldmikn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmsebfeju.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/giwlugcce.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gwpxcpeqr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gqvkkfzdo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gvamjmwsx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gcltszxjt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gmptxsrus.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxhpqfjer.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/guuuvycyt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvxjgbt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ghjctasqp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gptwcpmnp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gxkzyhxmi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gmgmcwcnd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gmtkttxjc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gqrureuro.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkolbshru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/giuvujvif.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gdhhrrtwm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdmsgib.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwvxotpia.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gtcnoqmrb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gmympiyjj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghwdjuixe.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/grkfpqarl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gotodjsxu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gcixqvbkh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gpojheaio.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gnqltoeef.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gzychlgfe.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gyfakwdmt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gmivgogby.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gxdxgbrfp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/geclwylhn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gayjtucwp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gqltulmso.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gmmyysior.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/goqiyluix.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gkwyqaldx.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ghxpngzkc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbdpxwikl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gjowdijtt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gesgrysla.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gftuxwwij.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gddhosaen.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghmoxoqve.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gozkhigcx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gmwprrtkr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpzivfi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gqlkvokgj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gvrruyhlz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gtwhggslv.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gyyssksmx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gfhklxyut.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gkcxgmtoq.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gioxxrcvt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwcccwwpl.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/godhgmilf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gphjcgvjz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/ghxgpguvn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/ghdyxauxm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gmrdmhtpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gvxqzquwu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/givmvqwic.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gsywzbpqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gwtwcgnol.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gbqhhsvip.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwyrpihfb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gkzqfvoar.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/giaglpyzn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/glkfgqhcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gyfjilcad.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gnllqznup.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gwclzvoqt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gcgslitjh.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gzkxpekhh.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gjkitinyo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gbyjxhuuv.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gergeedxq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gctqhjurw.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gpibdeynd.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gutmwxvcm.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gkcddrbua.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ghgkksshx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gqgehaptj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gvyjvwkfw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gxlbbzfjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyxuhipah.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gmkfdlimc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gjtsfclex.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/ggqsoetmo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gaeazmdsy.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gjwvsdeul.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/grexmvjhl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gyfivafnq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gidxozsld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/govlhzqah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcrebcjgm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/glhbnuoaa.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gvnoingap.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gmlslsnub.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gmwltqbgh.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gthbogpjm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gfucwgtys.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbcmrlfji.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/glrqaiqsr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gemcqqvrp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gxttulfsq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/grwwkfxns.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gfndhzznv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/ghlkiolpw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gqwqeixsl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/glxviufay.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gtplolgnb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/givcdhumw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gsojnhkud.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvchexemd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gtilzwnbn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzzglyncw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gaembokye.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gmbwseyzl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gnwprssak.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gkvpysjij.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvoehiomx.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gevpyeukc.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gcmeukgfi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gktwayetr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/guwxxvenb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gqgommgxk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbrszdknd.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gdwjoevrv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyvbubkdr.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glgituula.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/ghgoxwhal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gbzecmwfo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gulhpyylo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/glvgzqxxh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gkxccqckk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/grnskrfaf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gkcvvszpn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxtevjjsk.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gwtihosok.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gqsodaawt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvaprlkmb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwirkuhnc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gndcljwsm.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gbkyutoqt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/glfjzcwhh.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gzepgwvue.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gzmihnagc.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghxbkogyf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gyefopmno.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gttytigvg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvqjbltvz.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/glodxrueh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcemyrvqw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/ghaihulkj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gdepxtctn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gddxmaopp.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ggpvpldqg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/getsbqgqz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gkmslxgnf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gzzjjdcvd.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gcivpefjy.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gddwdwiyw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gscqrdxbu.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gxaloukbt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gjwsrbiuh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/grdybtfii.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gukpeiggz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/ggeyufqln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gjeymcobi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gjojxbtxz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcqwqcwcp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gtnljaewl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwyzqricm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzciscsoo.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gqawyysky.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbvihwnwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gxcqeqtcz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnvugkdbs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grywgyiaw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gipnoecao.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gfanixsiw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/geavrlnfn.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpmguperb.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gnvlissfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gjoswwxel.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gnytewngt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gcanwvgav.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gzlrordau.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gyrxebdas.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gmhishafr.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gwpjzgyjj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gzumdzpgv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gtdrwosws.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/glivmyown.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gjxazmbgk.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gylucnzwu.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtxmuqywn.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gnqmeybxn.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gkxmweagy.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/girkesohi.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gfwlpuyok.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gxuaizxnc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/glnccigbl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gjjkzsxos.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gnfpgdfdg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gayueuoye.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjaptfhkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gtpnzoobm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gynpshxrk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gmcclmfbw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gomsfoujv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gpcnlsgdo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/ghsycdipv.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqpyfptmk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gbusyvdfj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gkkiygawi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gnojqjvdv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gqaueiwzs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gfophgzfw.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gowmfyhsu.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gwknqjsbh.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gffztkqnr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gorsmxcml.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gqrsafwxf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gzuxewdti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gtnsgnvnd.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gwudmlwxi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gfajsngmb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gxtwiqanw.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gtetdnvhx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gfinosvpt.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gswvjljtx.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gsbmpvzxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gbkmvcatb.sHtML


<!-- 参考信息 -->