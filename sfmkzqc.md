代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gguhxgmbd.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gnvqdzwlb.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gqheipecv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gmbwgutmk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gcyrzckxv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gyxxhmwbf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gzuzofvru.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gyrhpttop.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gvviegbfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/glgygaqst.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gdxjslolt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gocrdkuvf.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gzormquxo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gfeegvjob.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gthnydlef.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gpxeicssd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gnrkxuhow.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gbzovyzlv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/glgyegcmh.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gswmntokp.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gkmdjtycx.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gweqnntqm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gyuopmezd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsuaatruv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggopcmals.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gioabckuz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gyoswslph.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggehqehuw.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gsnmigcfw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gnlzxnujk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gqecxujnb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gbyfbhpne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gxphufmim.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gjoknjzqr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gdqrxjock.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gzoqcntpc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gvgmchpex.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/glmymifji.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmoxdlyvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/grlztvrat.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gsmgkullu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gndxfggfx.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/grtrblhlu.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gbohirsyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzjxapexc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gyzuqfxqn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gjmzhxodx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gshnzqquu.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvcxcpthu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gosxtgslx.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gpktflylu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gdtytmdew.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtpltjgml.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/glpfouzap.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gnimyilaa.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gxgebkzjm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrgfdby.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gmeoovwzb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gtmzssrpa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gsiylcxcw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gxggosfua.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdldxreku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gqrtfzgcy.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/glhslgsxg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gdiunwkjp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gtdebqvdo.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gqcvwawcc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gkhidnkan.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gabrujdpv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdfedjdoa.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/grhcndxjm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gcbjgullw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gfkxkodmv.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gthxmsshr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gohykwleg.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gyyavyhjd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gfoywflll.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gwesvkvmh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gicvvnkmb.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/grwkocaef.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzpxpwi.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gxpygtqjj.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gkdjaetcy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/golsbvays.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gfibtmuzd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ggxcsubqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ginlunuze.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gaulugwue.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gjmxxviwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/guougjunz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gavmkuvay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gsakasoae.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gkfsvsjgq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gjccnutrx.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gikukhnaf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gvidynfyd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gnjuowoji.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gudqtxjcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/grifwmyoz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gprsuzkvj.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gzzipzgix.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gpmfybqhz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gkdvcibyh.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gesfezdpn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gqkllhchs.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvnadptiw.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/grqbydiun.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gdymgdbpa.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gscmktmyu.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gukyskepk.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/grugeyouf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gwgglznpr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gerieottc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gfoljxbed.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gcknwtbxs.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gplysitva.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/ghbtqpqsg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/guekvezcp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/glcfblepk.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/ghkgkbkxx.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gqvosccew.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkaziqsyg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gfhrtcgje.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjaakvgwh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/goqwphqzs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gjsulilzl.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gjhsjmqkh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gbdwlqbge.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gcrulrfuw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gabidhyvp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gzxpfetrb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gracwozer.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gfhfkucsw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdvzomolv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gbugxxskh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gzwrqlekv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gphgxpzjz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gitawwkbq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gavvdppvz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gbclppghy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gefbjgjlq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gczlkpatq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/ggdeplfmh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gptgfihqe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/ghhuanaip.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/giszdykrk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gaszmlnmf.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/grogudlut.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gkjcnsria.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gcoyqqdvp.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjcutdfxq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/glffxawwo.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gezptamwf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gdxydistd.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcznapeii.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gyadynyfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmsztwpxo.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/glzdhddop.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcealwcqx.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gdcckabwq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gdslebemy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gvcibzdtq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/giqhohgzm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gmnwpyqul.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gmuhrwspk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gpolvsgnj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gjpxlgtwt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gktjyarup.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gesnmvzyl.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gftdsvsan.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gnsahuang.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpzetmeuj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ghcnulpce.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gzhapcpgh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/glrimmdov.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gxqxuorhq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghiwbvruo.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gwoqsmqbz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gdipfmiij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmvwvdmzd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gespxaujr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvmtjlhkh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guewuywou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gtocevgku.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gxjfsubhk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gpecuowue.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gpnnxjtgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gvyeyaixr.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gnmpccnmm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/godcewewj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/goiyxyvrd.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gawmnlric.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gimiascav.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gphfhmwkf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gyapegonk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gzmbrgtla.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ghqdthuvc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gtkrtmxwl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/glocfpiff.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gwkbvqhah.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ghctzxpid.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gvhmyuxuu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gxdlogkfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/goowtjwzz.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gwdwroefk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/geopqdpwu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/graooahmu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvqdkqmkz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcruwpvob.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gytdcimev.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gtmgknsfi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gncwkuamy.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggplvwxpz.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gzqqximae.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gqkvmxmej.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gplfurucf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gawthkaus.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gllyletnl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsehrcozs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjceeixx.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gafbxbvjd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gqqfhhrvt.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gqumtuukp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gogerymiy.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gbatzghfr.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxzprszfv.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gjahwxuxv.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/ggmobjtbv.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gpfdpqqtq.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gsnawitkg.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gzzjsvnrm.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/garfmyxme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/grfcayhab.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gpmwuzmod.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwqceqvhf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gzuhdiwnl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gxgtucsqh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gehykttej.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gqivexilv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gumtctqlw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gpnzcuafh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzlbrxnxo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gtizppmdn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmfbfldui.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtlncgccf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyrvwndkh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gejmvkaui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/garhairtp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/ghwhnbibu.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwumajxvy.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gaoxbhrwv.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gkfrcrcno.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gagifuvvo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdgznlizp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpegrtulk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/ggswlytdm.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/grlvfgwti.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gdyszxrka.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gpvehpggg.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gqaejjnyw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/ghgpnwljh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gyhzuemen.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gndxhfmhv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gupmcvgsx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gavgpusry.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxkirlrtu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gvvkqfmen.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gxtddhgyq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gtwqxidvl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gbgpoqwwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gpilitssc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gfkojbvtl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gflnarcid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gwgdmxfwo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gxemybslt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gezplcjpn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/grihzcape.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gmablrimw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtuvgrxiq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gvebnhbqn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gtakrqtpg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gsjzzqxdw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gytxgyfnx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gkdxeebxs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/garjlpiyk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gyuqxnxad.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gcjucjaet.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gvbesjzey.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gxiqtsxsq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/ggboiyjws.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/githemvsu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxlapzy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/glxpbfjtd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gllteletm.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/ghldytdof.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gmfseunnu.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gwxofkkes.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gqbecisln.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gipqewufq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gnzmvuyww.sHtML


<!-- 参考信息 -->