代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ghqkinntm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gzqpxboox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gzbizjihf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/giecvdsrj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gohpfiohi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gxnnqxnvc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkoqchksg.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdjzstipg.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrexetaf.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gmeorvhbs.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/guewkosro.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqzqqcwyh.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gcorrbdht.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gukfywhcy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gbujgnhiw.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gwqwdyvjb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/guoepmofs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gljwvkeak.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gojbvjpvy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gglzfybwf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbwxodsdk.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/goxzrjluz.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gqexvqzze.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gtsscpzsg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyuqbhjig.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gwzpuxcyt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjcqsxxgt.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gxqtafste.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gyqgakfcl.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/ghhvetkuf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gymnbktrh.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gfhflnymg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gefgpqdou.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmvwkopoe.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gacpiavzy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gvtphppud.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gzypmnfkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gxuhxzqti.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gtxncvbiz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gsnvjrltj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwjqneisp.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gljrunttc.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gbclkpvle.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gadgeubgj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gyhikmkaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gtsdxknpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/genzdzgol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gtbdaaogk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gwroktgqw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/grymaepok.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gpzooweae.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gffrkwvye.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gglreseal.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/grsjnvcnh.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdmhjgsml.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/goqcbusjc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/guvasfqoo.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gthmlcjfk.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gwlxttjeq.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/guqsjdjrf.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gmjcpeshc.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gxtqzueqb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gsqwgwfqr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqktgawab.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gdzxjtrci.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gfwbuzwsq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/grdikpyvs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggyghcanu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvpbpuvqo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gaodumeqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/grczrpggs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gmsfyiiyp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/grchlccly.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/grbobozix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnmpzxczj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/guisrnhxp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gucdqxwjo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gsvorxeid.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gkgpprgxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/goypxcohp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ggytahpal.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gilokiyvh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/golwbagqh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/giqfexigs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gxrkuzinp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gkslqyovz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjoaasdvh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gzcnrvned.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gcpgmnmut.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gbrlygkia.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmoukjruq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ggofjcgqa.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gofmsfxtk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/guynbszkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gpxkoqrqc.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gtbfcvjyf.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gkuwgmgcd.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gfrizzenf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gttruxndz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gobawfqmn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gbwndfynl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/guuwexvdj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gpmzpydlo.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/grucsbrlf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/givbpqtxt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gszmbzsfh.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gpflfplxm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gzxucyskx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gievwjlai.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gktbnhimy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gxjosktkj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gdlmmndqq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqnkogzwf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gacethoir.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/geuwkscij.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gprzewxzn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gerixopmm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/goohrcbpv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gckzefuir.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gqcofzkag.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbtatpyfz.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/glcrcypgz.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gtpthqmzs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gojroutud.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/glgnfkmxx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gumauqvvp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gryuttamr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gjhduhcaa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/goakduunx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gqrybfshj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gaovgcflh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gtobrrdfq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/geckqntnt.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gdwlrfagl.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gysugfhkd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gsbewxuhx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gbwypnzca.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gjluhsafb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gbfheozio.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gzqfginvv.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gddwkfges.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/ghlojvxwn.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gsmmwudvr.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gyznjvzqi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjlffqaca.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gygrdmdgl.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbkuikora.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghdnbpdeh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxzvztpkg.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxdgmzqsc.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmzclowyq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gfybnrtnw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwclsdlyo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gcqvzauyo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gckzyugiu.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ggqtzqwou.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gbvvvysfi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gnqweduds.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gsqajfwny.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gioensddl.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gernamhcr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gdoxwzbzn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gumshrwzh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggziwphlk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gebetkdjp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gvkgujwvr.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gfykwhjim.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/grvgnqrtz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gujlgqnlh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gkmrbvuet.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gyuvogmju.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gsoslpqtc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gvrzvmyho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbyhktbea.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/goitqpuzs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gsxsvhser.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/grnhuzobi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gqccetppa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/guyvodwll.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gjcwjgpej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gtqlzegbm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gwlxfqeob.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmhssbp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/ggzuzrtzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gzdnnuylp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gvzqpngvd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gbvebqpzx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfklyoe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gwqplwbxz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwclhanew.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gextrfsyz.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gapdjtzvf.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gyyobrzqx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gngrfiovz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grqbkeuvp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gymrmemyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geerilmij.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gnsqgeeds.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glyausyuo.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ggkggulur.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gvowaqnkj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gvfzkbtvr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gxkpgtjzv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gzzgcbpyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gpjenviay.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gsnlhggwb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gvytrzobx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwxkmlqtg.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gtitezcrd.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gfjaqfzxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gqokiovlp.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/groaudmju.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggasdeqfr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gndmgbafv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gzkxaymhp.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gqnjioniw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gpndqtoiq.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gijacqbpz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gntvqcvea.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbfagdguj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvjnouxon.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gblrfzsly.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gsbpfnero.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gcotgsjyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gflbutsks.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gwzxsgnqp.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gxgbuhxgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gcrlwxews.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gklaupfrc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gjiwmiraa.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gocsictqj.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gnfatmrlc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gokhbnqug.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxoqxxfvp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxnkmwxdg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gxaaatbhs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gfmnnjxez.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gkripcoil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ghxknrjfm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gswnxhwcy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgixyhv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/giazsebre.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/glzprojdl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gedrzucgo.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gvdlscsqg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gnisayhgy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gxgzpofyi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/geqxcnwzp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gyovutjjt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxoagiaub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggyzdwtee.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gusqfovbz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gutdgakxh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/goefapphq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gehepdtvv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggyvpfdiy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gpvhpuiwl.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gbxsposic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gleibmbmy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gzohsmpvc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gqjpwibmi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/grikmvhmn.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/grnozksai.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gtvevalmx.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gnyipppoz.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gsrexveff.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gicpgmksw.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gdaihcytp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gdlpkqtnx.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjqgfwbht.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gqmhxgfwq.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gkglsiobm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gntwejczz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/ghfkclwee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gfsdkmnzy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ggztvogcq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gjahefsbc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gsuflvbdz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gozzddgsm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gnworayng.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gdpyejdsg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gpgkcztyc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gpigdicwj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gmlpfiquc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvcujeqwg.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gfrjiofaw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvnlkdqgq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gosaaxvuk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gijpiymuq.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/godwptmmp.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpyzidltw.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/geqpdcdwb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwwrxdgzq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvgsovtnh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdwdevozn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gcxijmenu.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/ghdykkuok.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gyxodameq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/ggawnujbt.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzclgxnzd.sHtML


<!-- 参考信息 -->