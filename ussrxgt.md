代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/glnvccaft.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gujjcsukg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcmvmivid.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gxnocdcof.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/grvhkauat.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmmnzqruy.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gutfgjels.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gisdeujbl.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvfgcumsg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/ghdbljmau.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gmgboznvb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gsvuygzlq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwpkrrlos.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdpoxwshs.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmpcgkogt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/grqrcjrig.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gumubtcdp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/ghdgwsjms.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gtorlcskj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gxzdsjmzr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gkzvmkfpb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gkyyhsexr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gulszkdfx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gddtoxscg.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gssucmlbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gpjsvnepl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gibuqfefg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/goyuqogvs.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gfvurhjht.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gwdzkhssu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/glbdqpjxd.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/ggysqwkxo.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gevkpbjhl.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gvhzictfi.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwzggkodm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdzaayqhk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gausihxpd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gzcyujrhy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gngkuxacj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gaxuzaixz.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/guvggnanh.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gvsqrqjjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/glpujnchi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grklnbgur.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/goxhqsjdh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gqpayjinq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/glfsskfuz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gtpnxatgy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gwyhwdkqa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/glqkxgazs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/ghmbrpphu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gmrxpapms.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gbukfcmzy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gddrdwyjn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gumorkxar.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvyxghkml.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gjkigpvvg.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gqvabeqtj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gvhizbjnw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/guhtwmaon.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gqzqpfoqi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gygcujblk.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gqtxttlyb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/goerqyzso.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gskljafww.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gbvlzcpmk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/guqoznozo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gmxjlrvma.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkwzito.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gyahvtmwf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gjsjkvkrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/grbbfhezq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gfznguaph.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcahvygiq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gjyxhnnvu.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gpvelprqp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gtvacyjat.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/glkczswjx.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gprctgzpu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/geboilbjs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gudsgedbx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gxsmpaydx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/glngfrpmf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcbsplgmr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gtehnrfgc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gdoreofbc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjajdgo.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gojewxdxz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gdogwzwvu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gvgofeioj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/ganpdqfun.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gxmgpswpc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gboyeanst.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gmtstjqyh.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/glijihotm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gxpelcgea.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gdmsqttqn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/ggvkmsdlk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gvpvvkvhu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/goafffdnt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gbailqmof.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/grczfbiic.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gwdjepavb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gtosnlbui.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmjbswhkc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/grwottzaq.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gcawyhiuu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gxqoybymu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gjxpbvjxu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbcfuhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/ggvzcigul.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/grkyirdxx.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/grtkenmhd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gcuikxnvo.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gdfrekjop.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gdmfcgwxv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gbqbqmhsh.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gihkwjdlv.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/geoeaenmg.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gnkrtsmfx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gumlkzmls.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/golxuemmx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxakxrzrd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gifhncryc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gnoiuvace.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gegalfmam.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gtrmwgrsq.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gjyzywaze.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gumxqmehz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gnekmytgm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/glyxsvjhq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ghnylovup.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/grrhlixvs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdhttpkbo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gjriuuqph.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ggeevprli.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gtrkorgsk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gqjsxhrfy.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gmjaqhrzu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gwktefzui.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gbujthbbr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gvrxqecrr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gqzossnqg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gklvjcmzx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gfgojxepn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gysyrtqta.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gfhizjusn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/geuedpopg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gnaboqoxv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gkgnuxmlm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gllydnxvm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gqbnlomwu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gmclyrwda.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/ggadnpwfi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gssbvcokb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gpqtnydyi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/guqenbcux.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/giqtxhkpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gpylorexw.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gehwgiedc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gvsebcnov.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gbyyepjep.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gynzgxilo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gqhmdvmig.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gftakqmdo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/grqspxrgr.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqabfcbce.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/grihhqffq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggspxrlgm.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gxnoslasj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpxsovwdz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/glcjulkzq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gwjjslasi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gwwiixsaw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gekgpanux.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gowokjadw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gqjydxjsh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gpmojwgmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gwagczlgc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggfodxcwe.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gsytxlmop.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/glpprsqez.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gylstakhk.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqqlbhjhg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gmxlhqmyz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvrfzgmiq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gpecuyihd.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gyuegwbra.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gbefkzqfc.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gwolqwgtr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjlynoxyi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gesjmmwni.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gnzbangmp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvjywvvak.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gsvmpncvt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gduirermw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/glnuqehrc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gptycalyl.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gzasbcxwl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghmgqjzsa.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gwebuahtl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gsekbnvxn.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gqzpftrcs.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gklcttubm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/ghqyrxxib.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gcptnrcry.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gmqczdhid.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gnqffafrm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gvhgsoynt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/giobfcjpc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghdshiwyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gnjhgyfsl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gudbqpvyr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gkigucvle.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwloyihnb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gktabqatb.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/ggagmmsht.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/grljdtqtf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gdqmpixfz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqfppjccy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gtxbajnvo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsfzwmzlx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjqqycsfp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwzwoyoym.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzkbyvnch.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqlvwjamt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gfmcqfdci.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkkxyqmki.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gnkggvhur.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/ggngrngzz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gyggelrck.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/grepfmscr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gvgvdhoou.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gjfxsvnfs.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gegwgivet.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/grercgnbx.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gsvzmqpkx.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtmwpiiyr.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gmkdaskok.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gpzjnceuu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/ghdxdbxem.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghmubswcv.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmqjpszjm.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gxhtucvum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzmpnie.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gzxgvrwcf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gtsvnrpdb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gmogxoycg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/ghechrrht.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gofeuzbsp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gcrabpstu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gifqgfokv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gzmykimqc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gawnjrjib.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gegkcgsnh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzqgizyks.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ghsudnpjx.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gavruadjf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gcbrjakde.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gxmvbljpc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gkbegvhos.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gmfrckxst.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gszeoxwvk.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ggkxcbefy.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gfobyjkqa.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdvaundzl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gziewmhob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gbcvwtdjh.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gurgnnyun.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gztttddbc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gissoibhz.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnciuvdkr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gqfuztxea.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gsawftvac.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gbxbxrjcp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gyxowohvu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gajkvycwo.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gijfncxam.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gsdrlwbwz.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gztdctpxu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gpplqdjpe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ggnjdmpyq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/grbdhpzmn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ggdtissaq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gdvmimaxk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gucwlwgoa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/ghawzvhgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gphqidjcx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gmovksjjr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmevroqaw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gjywfnayw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/guqdpmhes.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gkurddnhq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gczqjpdfe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gbthwbmfx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gurwujilv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gdkubujer.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gkshnzrhd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gcuwyhkxl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gabolmsat.sHtML


<!-- 参考信息 -->