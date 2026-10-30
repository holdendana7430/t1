代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvheqlgp.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gygmdxjmj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzqghble.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/girbhcqty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbcujpds.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/geleuczkq.sHtML

[D09] 排序（升序）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnwjajds.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmybpefdz.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmjacgaq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbtdzbxv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gaubsxfwz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwexjzzsw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggasuxume.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/ggelcoldb.sHtML

C#:   list.Sort();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtacqhfqz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giegxuvjp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizopwvtu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtseuvxyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcqnyxjg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gewiwhgrh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsjxjxhg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddktyzoi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjttpyfzg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gokrfdzoa.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpymzpkh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/guskeccec.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbnqalen.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/ggzachsmw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbjszkpg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwrocusy.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqehnhmsr.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjtmdnbh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhhrqfd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytnnotyw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gkbgtljci.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysxojnyn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsfuhzabg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/guwuxbtsu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcdiudpi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfaddztz.sHtML

Ruby: arr.index(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwoyypak.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyisrlnk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gyocjosed.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/giqollkji.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvujlhyic.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdotumnwl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gnqowfocb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdwsffljk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpcxtchq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpkoniaf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gakjmrsfk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gcqutfxxu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuykwtqg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ghyanuncr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjdwzlfu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsravvjvx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqtwxfkm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxqbrsrx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gaplkgasj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbptqbyr.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/goxminrvm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gctxbxyot.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/giuibznco.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gauhxhiku.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzflmycx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gqgswonxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdqusaik.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/gpzivqsfx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxstlbph.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxfaovwj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpptamcq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgfgyqz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gitwasdxi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkefkwaa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoehevha.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gpdiqqbpu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gysdhensi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlbckui.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbvatnkw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrnlrfjz.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcbtrazde.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gktzkzyke.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ghapzvsiq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gaqgqssrs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/globqggrd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gygnmztfb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genxzoxor.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gxruycouh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gkbpqexqx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfctojur.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gorjnibll.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gybocyial.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gibjspqkd.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/govfxztfc.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gfevjhylx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gtqzqqwat.sHtML

[D19] 按字段分组
来源：http://blog.fanxiaobao.xyz/Article/details/gjtdazmng.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbbkqtad.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gysccnycv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnyadlmt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwliwltd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchnfwenx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gixyfwivt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gicmgkttz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/galmpduzl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyjsixy.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gapnxjuyk.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gghzmqnls.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/ggccjbjqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gnenqxvcu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcfagdng.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzanqswv.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjsimwtd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqjjkhwf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzhlhxzy.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/guervvxnh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzknikd.sHtML

JS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbmaptcn.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtdavkbxw.sHtML

Java: list.contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzrrtfkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmghoruus.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhfmmphu.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gernefkzo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsiabkrt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumkciop.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoqsuomj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgsimadz.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/gacsomhoj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuavltrf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgcifzcc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjqpzmhg.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhpigtoq.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gtbqbgyyr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeolxbjq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfzmlkxk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/glijwclbb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gpxnltsvx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemddtsrz.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gedrozefd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqagwedz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvobmcarv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gisphxwam.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/glfkxkngx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gaimviunf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gelmxtwba.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptsqgxyj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyoggusa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gljpoijjg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoprkcrh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fanxiaobao.xyz/Article/details/gmgzukfym.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gtbetmost.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gkzbulpyf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gjnqaaxen.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gavxnjewk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaunrsyt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvepehku.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcggxheo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gemofykvp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpnozdzlw.sHtML

[D26] 数组转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyxukwub.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gothvdzyl.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gzjdagvpn.sHtML

JS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gumdpqjno.sHtML

TS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gmzupkyrx.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwmrvesr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqymaxutc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnmothmj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrczcqfu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqskrbpif.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwchavlu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glybqmrsu.sHtML

[E01] 拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grqasqade.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gucnvzozl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/grqblgcok.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlhldgli.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/goemchqbk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/grxrgofsa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqrvsys.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxspujr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/glkeypzcu.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmdyplx.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gsuymiuqx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gikmdcspg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxdquudm.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gmztqspxi.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggxdfjuuz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvgoaezp.sHtML

Ruby: "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gkjqclakj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fanxiaobao.xyz/Article/details/grqkvqbpp.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcxhyyyu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gthecrbgw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlgkhxv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/giicqpzoa.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/garhpyxjg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyvrhsvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gipsnbgdq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/gyjchgfad.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkosdmrh.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaneknmo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukthygm.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fanxiaobao.xyz/Article/details/gezlhnxbu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvqnofeg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyveotft.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gepakcour.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnetnupt.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giarxyuec.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gixmypnyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghzipbsq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gecjczshu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gdgnwzqti.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/geiaiiyei.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeduwejo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/grmhaudlw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fanxiaobao.xyz/Article/details/gqhlqkllg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfigonhth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/guoxywcpc.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjphrajhn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuujhihl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gvbvstlkx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gagtusatn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gouqrywkx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxzqigr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwhuwhtb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gjhkljpyd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxvigevs.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzonyarq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fanxiaobao.xyz/Article/details/gywiexgdz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkebdimvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gitwsuucd.sHtML

TS:   s.split(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjlmjuxy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/gupkbimam.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geytpmkex.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fanxiaobao.xyz/Article/details/gvjhqqezz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcujdxhwo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gwfvuprvd.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcecofxet.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbykdmut.sHtML

JS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlwpoedt.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqilboifq.sHtML

Java: String.join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/glbbzpslj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/gejqcwqup.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmglxeuh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcljlxrl.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gzesvnxco.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gekrlfgsl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlygfplg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgeaxppc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedocxrpf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdudxhauh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giutpkesn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gkmhdnnkb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvlmpia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gappgxkle.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gbqdehynd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbnycywn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gyijpzthq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdssglmt.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstuhvixf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpndhvdik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldzmbyxx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsldicksw.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/glcxceyur.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gldcqewum.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggswyktus.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblwwfjbq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gnffamhhq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/ghkxmkoct.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/ggusijqtd.sHtML

Ruby: s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gkspjtmcc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/ghcelndge.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gvdrwfvat.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gavwyhvyz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbqxfkt.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gryoxzejg.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbutngezg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/ggjruauem.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtyyyphl.sHtML

Ruby: s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnxzbxrs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeofmptk.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxehaagjk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbckdxruh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gayeaycxa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpaqolxtz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrsoeqos.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsqcwctcv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gvjvnnwxy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdkwldlj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gylqrofft.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwifvcpeb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gbecvjmzt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlopecpw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvhhtorw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwmhrepr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gxbfeqgvm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpzpkboj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggggvunon.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtfgnjts.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqunccobk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhdyudhm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdabsmaqs.sHtML


<!-- 参考信息 -->