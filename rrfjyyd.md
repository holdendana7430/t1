代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbbpneoiy.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gbaqpgniq.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gkefbtvua.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gkacxensx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/glnllwwna.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/glfydqscs.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gmqzmrrmt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gvmlmjmwp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gwlpqxiyr.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gabsnocmh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/goapwuotz.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gtbtjfhui.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gkkyzfxkm.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggubsswdd.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gmeuhjwsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwjsckfqr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpknpby.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gmciiwnmu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gkjfixxpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gfbsyxfco.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gvzdpydyz.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtkapuflk.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gddqzymnp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gcitwieix.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxjmvvidy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnygpbtfe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gezzkojuy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gvxhynaxp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/guflwpgle.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gkpkzzhae.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gxslenmot.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/ghsxwmceo.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gciitfgwo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gnuseofjl.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/goetpkkcm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gtpvfoouw.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gstbblpgy.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gqafehtag.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gohllkvri.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gnwqjimlu.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gecdvfjbk.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gmljnfory.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gvibommib.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqxobzjqv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gjqfutuau.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gslhzqlam.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/grfonzbvp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gojwnlszk.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gnaryravv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gczndnmhq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gxvfdpklh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gmjmpoymv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gcznfztew.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gwcrnvgqp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gicnljctj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ggvshxaal.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gvkxzomuo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gsnvnchhz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpfpcwumu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gvhevbznc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gvlradzcz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnxrojwyn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gcckmgfps.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzlagigtb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gtpuqzuzg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ghpasaivh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gbrrepevh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gxmorvuqh.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gvllfaghj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gygxeizrf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gapukjhkt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gzjiapwvi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gzqfxtqyn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/grqclffmy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/ggngcccyl.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/glifavuiv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gshdwmzto.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gkntobxvv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcaisazbz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gyxfxsiob.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gajsqodof.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbdnzbiyg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gzaqtzqon.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gmsfblwwy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gobsxynww.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gglupvexo.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gyutofcmu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gdzkviowu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gcjpvdmpu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gzhebftvq.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gthrevwmn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvotwwouy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gflzjitmy.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gudawufwi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gqzpwiqij.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gmealbxbr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/guykwreck.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggnyhabie.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gychmmwbn.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gjetxpcpj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gluyiyvfa.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gqkmsvefj.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gactocufn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grgimjtef.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gwticstcy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gdgsvizyf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gprsxxrif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gpypdabzr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/guprozram.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gdsxssszo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gvavqvsyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/ggincgyty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gtxkleazh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gyozvlggz.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gggugtxhh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gslzwltzo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gsvdglbaj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gnnwgabvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gytoyqewt.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gulbfczts.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gfkebjieo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/grrppjjzj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/ggvpxhqgc.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqtqvthmg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/ghkabyhya.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gedfggqde.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gnsohcpio.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbprevlbz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjizjwarp.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gowhazwso.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzwiuqyhq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gbupaefpr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gedoovsva.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gcmiappim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gwrlpwgjk.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gfwgdqwvb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdhoawvyw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gamsxudtf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gdoiozhzm.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/ghxjclxnh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gyqhzyivl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gacoyppds.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glldewkcv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gpexetchp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gtcjavzmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gykglkgsx.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gwhugiybg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gqxsvqwso.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gnsozobbo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gfdwkrunn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/ggsqplgzd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gheqyufen.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggbyklcxi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbdnavsuv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/goaugdtcq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gjknylqxs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gvztpwxfn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gdbfooijp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gcyehgdpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/grlpdbipk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gmclqbfnw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gduantxuz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gasybtyyp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gioohxbvm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gqbqrphjw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gqmcnmthp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gipqxzwaz.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/geytrhjky.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdhgmhnip.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gknnqjlcx.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gylntdxir.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gatihhron.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gdhlvoyei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gerxodjqk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gaomxsrme.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gosmlincp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqcexzjgk.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gjcdeqiwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggkqfbkgt.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpbqdvekm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gqdlkrkkj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/giqlvyqts.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gidppgoaq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqnkuaqww.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/giavzzfrk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gcrpyibvc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gnfmozznv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gurbkrdqz.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkfyyiyhn.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gmhhajzfu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/grommgexb.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gjpmmffyg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkimwdwgw.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwvkiigbb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gsqoidcob.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwsdrmjlw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gxsixcppq.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/geauppeiy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gbadisjsh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/girwvmsnq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqlmcrvjp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gaqatzjaf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkvjyxkbv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gktmwjgda.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gpttkcqjv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gdfwmhfrv.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gptpcsldp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gguffatpt.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gnhrpwgfm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gpzxkfwku.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gktdfsjrr.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gvywixzon.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gspqnldoj.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gdlykuazc.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwffszohi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gbooskbmb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdjbyvujn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gzrdfllsa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gyoqhdvoo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gociuzgod.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjyzpynwr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gcveacpvw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gkkngiodr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gszearjbf.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gkyysyudz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ghznibcze.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/godywmjew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyauhnxoi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqitfpyq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghwmkolzs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ghkonodhb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvlurlref.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqzcvhuhq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/ghyzidsvw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gnehdntdm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gupvkgfei.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gugtbkjfg.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gkomgahjc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gtacyvipy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gpjottcpn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gvgrwkpig.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gkbjdvriv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gpikebrac.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gctuaugey.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gnmjyzrjl.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gszrzrzyw.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glptrlofj.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gobrqdmwu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gjulykeqq.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gjttumwrt.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/ghblxaecl.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gxfvqyzez.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gttnvyajl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gqdlfwoxr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/guwptpmdl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjwbvylty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gkxlxvkzc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gtqzzcveh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gntytcisx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gnbojuahk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gvbsmxtgk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gptnlfmkc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/goixnklhb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvtiugrbw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyzzegfhm.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfvpafzvv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbslftdzx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gfvawkaac.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gqtlxdncc.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/grkzdzkni.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzlolxmtk.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gavwoehvm.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdiyhivzz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfbgwrihy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gtvlbxwhi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gmqbhrtwy.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/grcqrzmsp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gsurucjkm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gojnanetc.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gsidoptfu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gthbrftnp.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gpcriffnr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gkqcqidgy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/glxxhedsh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gvlkrkfrm.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gzqvllqmh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/giwraaost.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gnetuvyom.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gtpuvpjkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyegfuwu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gubojthes.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfnnwpryv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gyhdvioha.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/grqvdptza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/glfivykok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggpzddmpi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gsiaaqlrn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gognwyhik.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gmudibsng.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gmvsbqfjz.sHtML


<!-- 参考信息 -->