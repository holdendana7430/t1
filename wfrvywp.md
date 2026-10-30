代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gokkxhqiz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwtdeligq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gppnaxysi.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gsxnmipqe.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghtmofwoz.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gyncjzmhv.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gczeyhoip.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gwsbefxzh.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gzrsdqdjz.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/glzmrmdmd.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gppmkcirf.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/ggkhcimbw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gpbzkdwuo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gnxmbxqod.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gzbpnnjbz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjwwkgeyy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gfhfrxjid.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghybdopiy.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gvimzxevv.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gqskropaw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gxefhpspa.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gtkzskyhx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gahgxyxcr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gvpcwuxsx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gnmxnswqu.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/ghxehasdm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/grguhqrfm.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/grzlhsjru.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gcqthqwet.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggccmyipv.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gccsucexo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gadccxluh.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzjvafghf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gkwfvicsi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gmdkiqljg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gvgyogqlq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqnphtpoi.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/goqceoxlp.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gcelnbgig.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gevwfecqh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gxgfsapqo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtyeagjgn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/glkxtgabx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqfjplecn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gzbrvrlwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gsfpesiwo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gyypevgmx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gmkybkqwn.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gofkfulcw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/getrfuoud.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gsxoaikug.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gkwheoztb.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gvijzzncv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gybkbgfgw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghiorobfq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfwgqqr.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqyzegxzx.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gpzmtwhby.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/ggzvwmiec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/grydewtpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjveykukf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glxdwwlug.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/geusrnssz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwcqkiskk.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gjldtpbub.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gidyrwcyp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gnieyswvj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gzzjdjlgc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/grndkxcve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmwlteopx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/ghbjgeqrx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gvyflsdja.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gvzbgllvo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gixfnqatz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gcjbodsdd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gbaxrfrwv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gxsginkza.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/ggownsqen.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gbvbqmmpg.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/glvhghjkf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqlaucyqz.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gvjwvhknd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkpobzywq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gegnlbwuu.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gybuhpucz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/grkvbfvtd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghnraozlk.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gnsnnygtx.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghfuqkdju.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gqfiqpeyi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gqpofhjen.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gmrhudccp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/ggqeumdzd.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gtkaptmfk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gigsdfdlk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gnfpjqwjs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gktjitnzx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gieiudqnf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gdpfmwnxe.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gzqjwwhob.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/guolrsrma.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/ggwzsebob.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gjyvlijom.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gkpxyrloh.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gajssfhax.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtcpbpjfl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gponbfqle.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gmuycdgch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gcbkfiefq.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gyougwxes.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gozxuzvfw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gpjplixqs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gzrebunmm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gvokzldnf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/glurbzehv.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/ghvmhfqnr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gawgqjjjk.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/ggipqbjco.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/guhbcllpt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gvswyoqns.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gwcguklyg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gkamazyfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gnalfumur.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gpwbxqghe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxufvrjez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gdumsmzky.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gguysxohb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gplmpzkpy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gkopdfacu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/goulywzud.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gmlutfqya.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gexfmerqt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/ggfykisgo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gsfyegneh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/geigtazsa.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gxvbwieta.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gyaurrzal.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gxufyeeux.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gxvhdvzlz.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gkmyqdbsx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gxqeykpvx.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gcciodpsa.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/ghdhpesem.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghpcfmzly.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/giephmsyp.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gtswghxjr.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gcnwgliuc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gzaaxholb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gfkkvlcjm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gzwrtkywh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwfmpfnme.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gcldzwfxc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gpjrymwzz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghmaiauqj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gdnbhyspd.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gzuflwwtj.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gnlybgoxj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gieamscjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpwwuhzne.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gflwyooep.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gliahhshl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gjpivfnrl.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/glitwnaku.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gcurhabbn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gcfunswij.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gnkfyqvyi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gnschjsrz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/ghuvittui.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gzoqglvmk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gktghovqh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gxxqchxhk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/getjpthzc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gqmmzhqeg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gdyjmjnii.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/guhtmdeyj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gubuvcleu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gzuzvfddz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gixypwcim.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gaerosyoe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gpypalzkr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gecxyveax.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gilytutmq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gdkiingws.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gudksworr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfnwjmmen.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/geloypgku.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/guopbgxqb.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gdxdtgpqc.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gjfmjqunp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gsiksahlk.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkhaowghu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvgcbhca.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxflhvcto.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gqmvhrbhd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwcuewovy.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gyfvifara.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/goupfbotq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gbtbvnosk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/guvxqxhks.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gvnvertag.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gdhirtkuz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gxwalinpn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/guozngxgf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/groitrvvy.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gasxwoceo.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gnybxbeao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gewvjlghb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ggjmlqtbh.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmljbwumv.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gqpqvuypd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/givfakduo.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtqajlvcs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gjxfprcnd.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/goqimwypu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/grlwqahln.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwvmispif.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzuzohiuv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gbqbfuihf.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gmylugzkr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gfphxdkcn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gqjglxueo.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gxebzxvgf.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gyvajsyxt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gkwhekpdr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/ghjjaazpt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gmoxfvnyr.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvtjnundd.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gzuqohsuv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/greoaqbav.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtjtuwnvx.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gegrqhetk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/ggdmammkk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gzcwsrlbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gttygpfot.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxzkxmzee.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gmwwdkdud.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gwbvbeiqe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gcusylkdf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gkmcbikdg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghjqwkyyq.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gbhtrvvxm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxgskqaav.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/grzooxjld.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggtrpmhql.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggoszixsr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwctyuwrn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/guwzrmuha.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glbyqiocy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzxcrzvzr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gmfcppkec.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gppklzutr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gdmulhbty.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gbrhpkhcn.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gxrqcadvu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/genywjtfy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkkblzvpn.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gxvwzbeyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gdbfciyqf.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/goxicbsuq.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gdgbobdsr.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gqntcwfdj.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gpnnvveau.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gcapjvubo.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gnawngssy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbucdusb.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gtxtvxpsc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gbyyxjkdh.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/giphqknmn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gzqjcxlke.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gbnrihhnx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grmzgdnaj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gtdqnongk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gmigviazd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/giertiqyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gfifhzqfw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gecrczamd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/ghymmgdwv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzaxouvlt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gvkpcsbkf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggvooyazy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/grjhbedpm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggxtdudxk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ghntxpjns.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gerfvkfqy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gohexhvpp.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gkgewefib.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdoqeeg.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gojivxmem.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwqdjmcvh.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggzteipcy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gbehjuapv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gidjnhmsp.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gilrvofyr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gcfhsuibm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gdlwwujpb.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/glmhwsmyu.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gcggxnfim.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/ghmcuuzgd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gllqnyiki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gasloztwf.sHtML


<!-- 参考信息 -->