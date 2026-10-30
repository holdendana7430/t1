代发 wailian999

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfygtskeu.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gcokifeoq.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gmtzvbeye.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gzkgyrhjh.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gicwizlvp.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gxemhxlmf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gphoaivmb.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gktsakexv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gtogaebvj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ghkllfxuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/grjovghfc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gknovqebm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gpxmtweoj.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/grpuzhdwx.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gxvxlofas.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gcwjjsfpi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gflitnmtv.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gnzebwaxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gtirykpak.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gjsafzpdg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ghuhrjrzw.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gownujsbb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gplwkhtlb.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gymwpaaxs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/ggxxyvwhs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gynmliefy.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gisdesiob.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grxwogajv.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gcqxrberc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gdokrebga.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gmcfmbgwq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gwosvufys.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnaveeqfx.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gscggggsv.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gkwmtjbom.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gdgobzngu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gkvqfoqrs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gogreytrg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gpcnomgls.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gxsunrrsy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/grfsfibhj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gzczkezmc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gcxqjhmfv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gvjvfsubu.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/guxzfgyra.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/grsroevwx.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvtbgzwkf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gionhdxrc.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gnanjgnhs.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gfxazlwqg.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gayogmojj.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gwlgsaeic.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gsoyhnchg.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gpfrfoahu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/guwktaesg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gxfmfyxdp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gakfpdfud.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gkjbdcsyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gdmvdntuv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggkohdnrc.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gauokafyw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/grdoipolh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gtnoqrmuj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gxgyzlzpz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gfnhycifo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnpgvnevc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gxolmpwxe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gzhvhgfto.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gwxzgyfhd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/glpjrfnhw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwziwfswq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gvuqfvanb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gehxizrib.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/ghfpapjql.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gqobgrcma.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gflpaobxd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjfhcspst.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gsutevsib.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gtnhtqmja.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/girwxoyyw.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfbrssytx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gumckiacb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gvsmkloon.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/goeavyxfq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gltwllvfx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gaasqmohl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gtzdaycyo.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gtmilowar.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gapfehccc.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gmjykjxqw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gxrdwvuxx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/guatgnbmh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvtlxensu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gtgokjxcr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/guegfjhzj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gptfqhrmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gdcdxonst.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gafyruges.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gcdxfmuxv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grifprylc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gutweuvwz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/guhfamjim.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gvowuhzoa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/ghitvylen.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gfstssubr.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gjajjhrxc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gtxpsbkjc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gkzjtibzb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gkrxeglml.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gknphnpeh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdylsfehy.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gqdlimzdh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gmpivweup.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gpyrorwfa.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gqbslqvfn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjhbgudhc.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gahbdkvlq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/glqqextsm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/glpjnngha.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gmrtgceik.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gghedhzur.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gufhuotci.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/guslchsod.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gwrumjfyx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gpunjnsci.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gxitrevfm.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gckskbskr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvxbkolmf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ghjijqbgp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gozdewmld.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gznfbpgva.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gptvagqax.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpevtdl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gxhfvpcvd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gnentmcit.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/grnzbuenx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gcmdifkmn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gcchohsjo.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxrhnpklv.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzvtrcpqv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmekfyz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gjqgeeacg.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdnrgqbqk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gbpxzycki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gfcracvva.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gyiyhfhpb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbedloair.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gbsqxvoke.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gohganpuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/goyciqnro.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gttmbschs.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/giplsqisy.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gcefsysfy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gbasjciax.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtrsrpp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggbamrclm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnqpvojqb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gvkxtqipq.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gqfjirxuq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/genygonhc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghamdarpp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/ggngppsbo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/guuppcrfn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gdwhgukqb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbuxtmv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gvkgxqlsj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gujenqqnr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gigfjyvax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gebciasjz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gcqwjeemd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/glbxwfyvi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gsoyhkqjq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gzqbptzjd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gvcwpxwri.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/grlboedur.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/guakhxstp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmhcuwfj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gdxarbslp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gkaswjcob.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gxqrijuwr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gpvpipedw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/givgymiru.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gulrwsdxr.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/guwxvgysq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gqvvxpfcj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gilpxksww.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gbejhfzny.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gfusewipe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gydqmrkgh.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gfruqwigx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gridmeica.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/guokorqlt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gmjmzmwuc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gmldundpw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqmaufrxi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxjsvekhg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/guwxrhzft.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ghgwkzypt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gmbkcnzhm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghqstbzcl.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/goonghumw.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtckmjnye.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjfbzwz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gristmhem.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gjmwznrak.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gbhmddlws.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gonnmxjtl.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gphjvnqwv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gvykmamow.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gtebdwcue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gnmbtkvoz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gqezwdano.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gjrazcndb.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gzshhhiel.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gecmudwja.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gjuxrteqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/grnctkeww.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gslbdbmal.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gkxnpysed.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gainiscgr.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gzvjvjbep.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gbaaqzzaf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/glytdxupz.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/giwfzrosp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gixmwvmum.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdzatlca.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ganurzcgx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gkssfaess.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/ggcrjabrj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gvfufqphg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gqcfwqvfi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gultbjpyr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gsrgcbcrt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gwrlmadye.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gwcjnxvsl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjjkjgabx.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gzevjdika.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwqozgjij.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gmigukmao.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghszuxwkz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grzojunjp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvtjwochy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gslaxpnlb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gihzlnqpr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfnejhyhl.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/giojzoabj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gcmmukgjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpdghyrkt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/glughlpzp.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gbuimckvo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gudzumyqk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/glcwwvnez.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gipkixsqu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gthlpsjqg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gzfdqcmrh.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gonfutlmg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjxvana.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gtmyastme.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gbiypflhr.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gqkdlgibf.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gxsecbice.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/geuvzjthb.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gzalcrjpk.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gwbswxdct.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gndbsbyqy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gptosnhzr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gagvioryi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ghceausbe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/grcqswfyz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/ggxdgwrdo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gjwezobtk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gibhskwpw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gxuuvmpbo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjhezhdfq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gwwucpful.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gdohfuipg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gwqhrkdln.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/grfzrknja.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grrnvnpck.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ghhvmnkeq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/ghshenonb.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gxwwrquhy.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gorafidxv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggjkiapgi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjckmaxvx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gocyjboth.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gojyytesv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gongpjdwn.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzpieca.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gkmnqxbio.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxyctwvxo.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmbbsrzgj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gmhyzdola.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gexlaawbq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gsodvmuwj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gbbklhaen.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gqefeigrt.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gpaxntwhu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gukvrsaqd.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gdvkbxrpk.sHtML


<!-- 参考信息 -->