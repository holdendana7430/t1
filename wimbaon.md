代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqqzzvvhf.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqdvygtqa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gyqocngos.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gaxrnjiem.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gbxqeciuz.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gwdqnoetd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gjqazpfqz.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gdllfsaea.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gntcjuvfc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtuornhoc.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/geqfhmnis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gtkqbxrhy.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gkgzydbcb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gzbjdlivb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/govufjndk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gzcrpluaf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gahmvljae.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gnmqbydee.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gugxvwhpv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gpzuizyto.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gemgtfxez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/givlqnbdm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqurlvprw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/glvwdlnyf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gvuzgogff.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gsjgjechp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/goykjkxzx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/ghzblblya.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gtmgnfqex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ggngjkfna.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gkkkwymqu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gldhyioay.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gmfvkrbgo.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gemjrrupi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcleckqhy.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gtrxertov.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggfggcwly.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gjazrhfrt.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gkxmaftid.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gspeydpla.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gcthkhrmm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxuqswbuh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gqukmwvbr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gddstyjcm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gckfzaqsx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gesypxhzy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gterdkjmq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gdnduagjq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gnpronfrx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gblyysxpy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gyzavkbug.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gzjxxdwmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gjrkokxnd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gmomzypxp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtsizhqgs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gfnnhljhj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gzblituac.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gvhnsqkbl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwioihste.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gkmxtbvzg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gwhjdhzgc.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gvgscivlb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gbmccgviw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gauupajcm.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/glszuwsfl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gupgcnyde.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gablflmro.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbnqzhvae.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gsqrbkwyh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gyhrjtujn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gvmhjvnsq.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gliqztfqm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gmxcjaugm.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gjmiqrvqs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gqhsjpkgn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gvrttyrbt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gjdrladzs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvpqdvusz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gwgcwjbyq.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gpypckhgo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gupyrcxvz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/glscfzdcn.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gxkcvyrju.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gorcbsxoj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ghduogciv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gucucrein.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/giygzgetm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/guwxjhpmp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gmpaqhzxd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gyurvykgc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/glwlznoam.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gjaobxizv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gcsppudld.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gywzcsbsz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gqrhocwgi.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gqdyhhjvl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbqsmzqzz.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gxhuxmlys.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gxdbvkwqd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfxcthjcd.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gueisntki.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gxbdbevxp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gpjqztofk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gvykcvxmy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gnlkgfuox.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/growdgati.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/geenvjhwb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/glodfvywe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/ghvsrtyan.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/glfzjpkah.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gahmlhnzd.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gkxuqobbo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gfgkgkihb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/grttphtxe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gmkwewvap.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gijztckpm.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/greiyfioz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gougibmbm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gurbegoxv.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/glhpmjiss.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gkvmjjfvj.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gscvtwllz.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gylpjyqkv.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjtipbjoi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gadxgyxwm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjneyelv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnnjzlfui.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gwazuxqon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grybyemax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gaulmdotc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gshnjlpss.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gywbfmgfp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnzxtjqol.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gbxsgcqnw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gqzjpboon.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gxjskwggu.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gdlvgibbw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpgpifrrn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnrdpalec.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gchkmnyie.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gwgwbhrqc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/grnkbmewn.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gojvzgcog.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gjgmcjelu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gtrervsjt.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gxzzdxysl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxuudayxk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gxexnatjg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxmsthhie.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gkeqfsrzq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/ggredivlx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gvevgnkkh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gggwrnctx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gzgrplruo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gznkzzqsv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gaxvdzwpi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/ggfhjskhw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjwbnscje.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gumvskcgh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gjmffydbt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gkotwpjbj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/ghhaiqxxg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gtrxvwdcu.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gkaczhrmb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gczectjwa.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gajbjcybx.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gzqufrgyh.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gxsjjuxnh.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ghwchdxyo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gylslxrqf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ggncouitq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ghlhxjmok.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gebdjaiin.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/glayqzybc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcamonwue.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grqetvzjv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gszdvqrxo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gzhqkxldk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ggnmblhlp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqcepzqov.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/goixkquot.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gwvpldufz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gsacqkaus.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gffggsqti.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/glzgoyotz.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbhgjstvv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gudqlvwxt.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gylilmzyx.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gbxbznbnc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvuytkhlb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gnijbheyy.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/godvqjofh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/grlhaooae.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gxygtlrzr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gktmnpyhu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gsdknmtzo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gafnxtrgm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gfqpnlcjc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggrkcwcbi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/geadzrsuk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gxieuwpkr.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gpwewhigf.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gxoajmrpk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/ghlnpjzls.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gkgurdeut.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gzqjmpmfk.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gesfwglus.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcsmggqfj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/geooqllcl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/guapbxrwc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gssycihli.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/ghfbwknnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gttnrvrln.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gbjffvfne.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gttxesupo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfsnzoaoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gccbhuglp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/grpcjqwcq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gjsfhjyio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwqfkfzvr.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gqkshbtuf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gwxlxgrue.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/grwxqzdxk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gryzcokxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyoitvfij.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gsizoscgr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gcrrznmjk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gweomhlgu.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvzziigzq.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gvzgnbqvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/ghjbavmtk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/grtaqmvwx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gsmyngvby.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gkmoafvie.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gyofkwjgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gdxlijihh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gnulubaef.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gnascxhsi.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/ghozynpry.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gufqmvmwl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gbocbzbbw.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gcnatlgij.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gtoxjotmg.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gogeqkqix.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gbxjnpkoj.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gipzhuntl.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gczxlhvdh.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gwshcwqlz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gtkycofec.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/ggeshomsb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gxxgbgrcw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggsrcnnug.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqawcqxla.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gwgyvphwx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxjymlw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gmbstajob.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gxavxhspq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gzudryprr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/ghwxqudye.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvyqnxmtg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtozvhixu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gvhafneah.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzfngskgc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gjlifublh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gkwjkstrd.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/golazitey.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gezvtdhgy.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ggkbxbwcn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gprbggzon.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbzdtkjxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gpojrkgiz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/giyagiegc.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gsfcsgykf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gzkyttalg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/galqekgmv.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gpynxkppr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gznwphopy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gbzossobn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ghsegqhws.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gtsrthhta.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrawjvw.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gooalaijd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gdaghrlip.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghhhtepxs.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/ggmmyplrb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gxwohqluu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gwzjozlxx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gqgczwdmr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gjgvsrvbl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwczayyik.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gxfynrbme.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gaqedjene.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gwxkywwvg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gndfqnljb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/ggljtdbbe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gmzzjdvzf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhirgihu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghpsdrsnz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/grtgxjkgg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gkaglbkcb.sHtML


<!-- 参考信息 -->