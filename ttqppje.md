代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gnyxonvzq.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gwmhrnplw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gpnvtlcpy.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gzcpmjlqv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/geynaqgho.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gyxrhdhzp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gadqapigv.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gsbdxigag.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gjjbwvssb.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghgyutaad.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gaurvpgtk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gmbmrfjdh.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gtuwawgsl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gcilbjfdk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gplbjxwyy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/girizpnnj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkyegkpmu.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gcuwtdnki.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gjnpyqurn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gluhhcien.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gwbpekndb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gneyvjmca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpegntzhw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghsrvnbbz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/guccbqmdi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gikmrtxve.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gllpcybdo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gqxepuzqk.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gzlascbiw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/giqbioxae.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gtlesaxwg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gqudalbvu.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gyikpujjj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gnnyusufh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvfybcguh.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gmrzgrlpy.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxkcttkxs.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gfzecsfly.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gtgtnbodk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gjhidojyx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gnhwydbxb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/glzxaqzzm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gtdtugftf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gaknwberx.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gqbcitxgw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gjtordboq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gtlbxfwao.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gbhrwmwxd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gzlumtntj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/glndcfxsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gthzodknj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gyhxwbjkb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gvzksvddu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gbzazqgjo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/goontlqpz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/ggfgixjtx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gveyzgwva.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gxauzykan.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gxkgghzuc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gosvamaqc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gahrstoaw.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/giukdoobg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwbocvyad.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gexboipsq.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/ggcvxrpwl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkhyffvqm.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/goubmmiip.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gyxmoqohf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gkqgtumrg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gtrwqukcq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gfdxktvnm.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gvabzejmn.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gelduxhka.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/goniqtruz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtxiexkym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdaywgqhd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gwzbajktk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gmevsyexa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gpfhwmxtt.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gfjaztypr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gsekwhftj.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/glnhaixef.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/goafhlzob.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gzbvozddu.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gexfvdjbb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gqoqcgsql.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqudkdet.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/guesznhqv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gnafolbqs.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/ghbxachcc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gdfrjljhj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/guzgzqzes.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gvzluzkwa.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gfjtzjfig.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gbwpmvysg.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyytzal.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gbeayhebm.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/guugiuavh.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gcmvwndqx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gddbnukti.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gohkvyncq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gsrszjaen.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gcluehigd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gbbagddbu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gueztaele.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gasbmxpbh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gigvsyxld.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gpqnqzztc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gdmqkqbvc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gnimstiue.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gudxfmmdp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gpomktscu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gujiacgjc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gwhixnywm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gwbjbdmax.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gzkrbmsal.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gtcumjtdr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/glhbjculd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gjgvixtzq.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gtjdzgdcd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gaokrzefg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gchcjbkhj.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gremfbour.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzflovefv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmbduycsx.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gfkcvpifh.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gtzxivtqw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gnnusygcr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gemmuhjah.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gjzziover.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gpdkmqfkg.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gdiqplqzm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gjynksfzl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gqmojstyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gdbffyusq.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gpxlqbxvf.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ggcxoklgy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glgupwqef.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gchpjwddn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/glrdgivwe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gbrmlfnmi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/grdvvzieq.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/grwcpnbnb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gfitdjzwu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gbyvhzrwc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcacmkr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gtvmtwzym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gyaezswhf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gglhyymub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gzdekyrhk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gpashmuqv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gjtyhflzv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gfkahcewl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gxhtpvipt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gwzfflgyc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gijfyctnq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gfeejcfcb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gtphejdfn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gujbhjjek.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gnodgukew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gfvhpiacr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gikcbohnq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gaeixuxqw.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/girsxyctc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gphlhxguo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/goxioiypx.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/grchegsbd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtgrszjvp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdsyqthbj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gtweyidfo.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gmpvdjuqz.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gxojiyuiv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gucsxqhql.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/galcunykz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbolzkwap.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gximobowa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gaihxergo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gzsckccxy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcqhirnvo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gcjnalgmw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfrifpjeb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gwwhcciyz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gesojibfn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdrlzivwo.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gnokbwuhr.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/grzfhdjyk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gnhzmxpup.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gbltkhyjp.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gsscssmbk.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gileksenm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gespxwaxi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/goaxlrrom.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gutcuhfpf.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gkyszzmue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gscnwplxo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcncijfer.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/grgvltdmu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gimaynxkr.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grypfprbq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gxeqfhjex.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gmtukwqrd.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gsfximsde.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/ghpbvhxts.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gielkxaeh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gqtiutzhu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gkhbboaqu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gcnehvpga.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gbsxbpbzw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gvtsijjdl.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gxlhnqfoi.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/guecblwns.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gyobdipju.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gigqyevnd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/ggbewsaly.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gsccgnvtx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gvrfxwkjs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gdplqziur.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gefounhms.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gtpjuuzlr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gkjysherl.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gffzbpobd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gorhaoady.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ghvftxtsz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gexysjglr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkemyzxgk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdcjslnow.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmvunghfl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gccsnbanc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gypwzjlvv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gzzbhmksg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gfibskgsw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gniswgxrz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/guucrpdfn.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gzssazvtt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/ggzcizfgs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gcvzwxroj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gpsmmptkk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gjhijwiwy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gdjtpcshp.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/ghydxkcak.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/grvuepenv.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gklkednvo.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdegckcnp.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gcuxjlkrt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gjlhlqpqp.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gsqopiwfp.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gkdrfvpzc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gyczyitpz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gawxvbkht.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gojwcrmvy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gtwfkgzxk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gpxulcurb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gkwmunrph.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/grwnyyffn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gevcxsbig.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gxlljcuub.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gixjfkvln.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnjsnudbf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gnoneqrys.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtmhwhblt.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcfiktgdh.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gpxjpmjyd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gpdjuxnmq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmmrberkm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gzkxwojog.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gnfcebrld.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwhtbwutg.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gzkfcdzqr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmsxhirbt.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ggpgkbris.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gecfcjcdk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gpvrraros.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gcncjxaeu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gmztdawkv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gkrzmvnca.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gggpujzmg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gjmcirmap.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gutugphsv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gialmjnvo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gpwpjkfze.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gsaetsspn.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gdzeptgxx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gzinnpqzw.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gjodvfbyb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gcylsjgcr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gkyuoeyii.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gapnmhtdk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gskumxonq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gzezxblsa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gvwrbrjeh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/glilgcucb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghzfpqndz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gxhknruhb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gwgkasvxi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/ghbwsiwiv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/githylnka.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/giqngiepn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ghftbgvet.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gnscfjupg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gfbihjwzs.sHtML


<!-- 参考信息 -->