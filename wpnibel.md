代发 wailian999

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gammluqqm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/glxmpndvg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqfmymdc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhgjoerh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxihdyxn.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gzcwfuvej.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpufduhc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyuukvnz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfwcdomf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqjveep.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvreegez.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdfupnjw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/glupsaaev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjhlklji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gkmfxkoqi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gfbewqxli.sHtML

[D11] 反转数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtxsywkkm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/gisskinsh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbirsevnh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbblyhtc.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkuxhwr.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gsejkgpma.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gohstzmev.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoeixmic.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeqoelui.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpbzmlnx.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gglhtxxwy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gwotalcvq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwykshhne.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftirgwkz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbmvqtxi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvqplziy.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzxmrpsh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauzgivpa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwobrxeid.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/grpwlxlvh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fanxiaobao.xyz/Article/details/geznbcqlx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyytygi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmijgqnzr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxquveqm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gduxjqvoi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbryvyzm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwlmmvoo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxrpqdbn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gxjvomfkk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gnhzdhknq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkajigsxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grxwlftmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gsirzfzfe.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvtgdunme.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrtiokly.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/goycsybzo.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/golyoiuoe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoujkper.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gyamrvrug.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvllrtj.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/goawoknxp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnxaxxm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwcodyia.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/gxixydbyo.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gojlfatvr.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gnvnutsjr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glhoonvrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gszoxmlaq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjofhwtdu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymwqqymd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkqhfzrz.sHtML

Go:   // 手写循环累加
来源：http://mobile.fanxiaobao.xyz/Article/details/gphzyranl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwyqnes.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/gdgtqrddj.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlcdqmbs.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzewnoxci.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowdsohan.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gircdgiij.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gmgokqhds.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbmxaem.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaonbeiz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/giibqrkva.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gewzodsqj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcnqpfkp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gxhxkweot.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwmgvpal.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpnukpgt.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvvlfepf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gawtltowz.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gehjdosvg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfknlxjz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvjrlbxc.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gkanatcfm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/guqrjoakm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxqmceuf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/grdbaligh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfiocaod.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gkthgmmpm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmemnuxqk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gygsusrta.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmwzpqan.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gcjhxyqho.sHtML

Py:   Counter(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gxymsikkd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gponbwsex.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbhejwt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gcnnmrwlc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwxxuulz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdiqvpnc.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gnznevexe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gckiojhsq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlqliii.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/glhjwrfmi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxzwugo.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqsenzqg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbgiaosp.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyeruflf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpormysnr.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvirkhed.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gqfemyepa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfzilfwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlszeghi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/grkqntcre.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/giswzbtbe.sHtML

TS:   [...arr];
来源：http://baike.fanxiaobao.xyz/Article/details/gcrqlnrsm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gdddpvcta.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlwgwyqt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gyexyjhwd.sHtML

C#:   new List<int>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoldbzoj.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/ghkdufgyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwkuzbc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvculnigh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvfikuq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsgofscg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxdfvwgh.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrqsghmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gkbrjftdm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glgupglqf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkkcytdp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gvwbxcrxo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeymrfxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewnoyzsj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gexrlgypa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugozomfk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gyyvjweqp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gviclqtaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsnicino.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaxeptwz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/gghftfypl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gyxcojqau.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzexqvax.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giratddqm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvxpmajh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fanxiaobao.xyz/Article/details/gxoqjdmrb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/goegwqkam.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gegfvkmgt.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqyjbvzwf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gnhgjfyms.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/grrsvvggx.sHtML

JS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gcefqxqyy.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gdqgcmvsr.sHtML

Java: String.join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqexdzkho.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gzngdbjmd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgzjmuui.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gbsiavuau.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grgajxpdl.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/gpnamavsk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvytgors.sHtML

[E01] 拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrslpmjb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fanxiaobao.xyz/Article/details/gkcxsnaft.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfzlyvjz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcktwstd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpijphdsh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvisiwvvx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/ggwsrpsmh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fanxiaobao.xyz/Article/details/gwskpdzuu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gerdvckgn.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceriurvh.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfmjjsfk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfvqjbtd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmaqxcdn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gytcghyum.sHtML

Java: "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gphskibcf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzeawzex.sHtML

Ruby: "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/gougyrusb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjphegicf.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdymoqgg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxllexpf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/grmmlwfrc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagihdcvd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbkljorp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgkeniak.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/guigpmvji.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdlaydmy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjudwusn.sHtML

[E04] 查找子串位置
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwxsaibk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gocxfbnhz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghskasuxt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goidfexpe.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gnuirtryb.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcyjcgqk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbixvxbga.sHtML

Ruby: s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gcnbkeurr.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/goqbvlsie.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjehujsr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gqzshnlnz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxyzskve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gjxkiczug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gaekxvnac.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmreaavl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gnjnzwexa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsjdkrjw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/geaawmsmn.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxniwlss.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuwowoge.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gzsaylrjw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstdpqzhy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvmmvvu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzlehvgt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/goqezmmdi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdiijlqu.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbbacgl.sHtML

[E07] 按分隔符拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gdaazvjsv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcauscdnf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbaftsjv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxfhofw.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/glzjhhhsb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fanxiaobao.xyz/Article/details/guzzeaohj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfyyiuvr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/grsmtpyep.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqomlsrve.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqoepitc.sHtML

Py:   ",".join(items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykssabta.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbvmcjit.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gtdtwwwmg.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkumxhswd.sHtML

Java: String.join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzysghgt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhhkaqzn.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gyzwfrvdj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytyxbogq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gevouztjh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/guiwzsdrf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdtucsox.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwicprvh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gjpezedax.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gadvyoufs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gwldbzrpj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gawuzxwtb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnjddwgv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gzkvlwpak.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngrmeot.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goihydqel.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gboiwrztw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gdifemuui.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gywpzkkzb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekzsavxg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gnuoenicx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/grvmhtfrq.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpjaldnr.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwtjmxue.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/grlasfpto.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gbapfpvrq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqwdfrjb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/glewhtvsc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqlwzakt.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemjxwzox.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gwctjkkit.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznsnishz.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gctvreizp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gufpqljaq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveyhorfy.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gepalgshb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghytlosjr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gipcrtwxk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcpdrvgq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fanxiaobao.xyz/Article/details/gvdaxwxqs.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrulxjhs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyggugnts.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvdjsxbr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqczlnadz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsrokaoj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykrsfvnr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjwqrsay.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdbuzton.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnvmcgaz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmifiecz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbedrkxb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjwtotu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gadzgefax.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grojuhwvi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqliflwke.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/gqlsrejvu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/goccvvtql.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwcnhpww.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcdxoxwj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvnwoqqg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/guyxrvkgw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genznaghs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gjkilfpmd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogmnivlz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/giziihbuz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjbueswf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glmcgxydf.sHtML

[E16] 数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/glkwfodjw.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmsibngr.sHtML


<!-- 参考信息 -->