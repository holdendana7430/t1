代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gwifzyymx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gunsmifup.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gcarinsxa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gwwczustc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gdypwombv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gimnvzwsj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gzeoqhwgi.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gwphndxsr.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gprjfluit.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbyeczkor.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gztnhqcja.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gubqgcikw.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gcdqgbdch.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkujztqhn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/glumvamfv.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gbqqcapdf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gxadxgtkg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gyjqnwdkt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gcxrjzxrf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggavlrbzm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/glswfytvf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gompyjzsz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gcankxthp.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gzabqhsah.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gyisapqbh.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gallyxtqr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gljsijasi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gkkflllvx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/giqdmkjai.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gkjrjkmqr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gmxqeyagl.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gcslajtft.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gygprbifp.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/geltlasvl.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gtyzfjsae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvbzbddzq.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gaoxyruei.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gfmtlxllg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gchlybfcz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/grrbleeui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkmwxldmj.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gbsebalcv.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gaqzbirxs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ghyhzgjzu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gzjjxxufb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gsjkomezq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gryvazcyj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/ggxizznaw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gnaatsewg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/guwxpnahd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gqakvdmft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gixwdmniz.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gpnzfqzlg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/glmwvbjer.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gkphviwlf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gobhyhqgl.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gcqgptvwk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gskqnjfyj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gtcjervxi.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gsfouqjnc.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gwvceizvk.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gprivzuon.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gtkczldds.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gqskxmwzo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gwkyundfd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gfkjtgixz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gnafsqdfc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gotzaphvu.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gznbnbkpc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gicswnaen.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gvdcesnkn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnufkclxi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gxuqonkgj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gmckllqzk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/guzsatfza.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/ghpzxumpc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gnkourgaw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/ghpvsvxbk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjlopdubz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrrbqyy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/ggtsbqzjl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwsoycyqf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gfmpbxwki.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/graxidhpk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grzmnpfjp.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpksyzmwm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gattmfmcz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gspxzxayh.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gpbyctaly.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/glcoizjjn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gjsmmtdud.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gkszmqtgc.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsnkekqwy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/govkuwhea.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gohvehbww.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/grygnblel.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwbvpxxkk.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gpcjnajys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjinksjrj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gtjzdbgjj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gskogawrb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gocqlllyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gtfgsxdea.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gpjomlxpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gzlnfwojc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gjtopwwew.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gavyrcgab.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfiyawhib.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ghebvzjsc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gbovkfdag.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gnnbivwft.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gxiolijqi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/glhdzcuae.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gojnkhfri.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/glnrrdtci.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gyhpsjdsk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gcirphvkq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gtzrjxdgu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/giowvxipw.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gwtybdqap.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gusayehlt.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/givfdevst.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gxvsncncn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/ghddpisuw.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/giaspjrtz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gmixvsnbr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gubtjcfan.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gcxqafzsg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gdctdhchk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gfvjdcbvg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gqefkdrhi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ghhzsopbv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/grixvpkoi.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gviebwjdc.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gspxdgoux.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/grykmjani.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/glvopjvef.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gglooghof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gehuptzxi.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gjvtcgndk.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gildplfeh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gcvkrvcza.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gqfjmxwlc.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gewdpigju.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gjsrlmmdo.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gdsyccpgy.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gihdvzncp.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnnvazlfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxukbajko.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gcjauocif.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkuoxzjbp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gqufzpuzi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gxkvlhtzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gnuvyvihz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/geewpswyl.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gjbdhehty.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gjiqogdfu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gfyhyarbw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/goctkzuvx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxexfxb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gkzqhumwh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gfzjyppou.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/glennvbxn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gthvnipwb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gkvfsmyhb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gfhfqpxqb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gcwtlewxp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gokacgcof.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gnrqocepn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gjkclbfsk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gipxoeguc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gmarohsin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gepgdnqcx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggltwdkub.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gdvvolkhm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/grjpsntqt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqsfxgmqb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/ghbaptuwz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/glsfnkutl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gninnxntt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gskfthxln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gdbfllycl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/guskerzki.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gyaadawqu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gqgcdsojw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/guxodtqlm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gsytmbvyk.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gubziwuce.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfamxsidf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gshcymvra.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggyifjadc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/golfejpux.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gkakdqlea.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/glguxzbaf.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/goorybrif.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/garmydudw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guzofxzjc.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gykopbaiz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gudunrabj.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gycjauhmc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gbmiazglg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gcbxaqtaz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gnvhfycmh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/glcrtcafw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gglxbbnpp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gtqkpsqvc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gppfqynqb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grojdxfhk.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gxtontfdr.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gitiopgrt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gmzwuswei.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gaehielnx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gpcmeguuj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gpfoaoqgm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gxlnopzlp.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gqspxqfyb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gqnooofbd.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/ghvydoyyy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/goifgkglw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvnomudws.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjzgvmnfn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghwxotffi.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gajllxhps.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gnpnsfnmh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gfmjoflho.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gdrevksal.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gzvuxzgjy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gfpgokvvn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gonxvzvzk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gvreivajp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjtqqoind.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gwguieefk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzyqpbrhs.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/grougsinq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gahlnwlgp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/giwghemvv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkkqmexnh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gvldeyama.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/giwjtztuc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gnwgitdzp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gljtyewyp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gchauldiu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gkeiefrmu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gptlvuukw.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gowjiajmr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwqjifeaj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gowkyjgvu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjsgfzztw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gomsfwqpp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzxslelcl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/giuazcnxq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkixlqngc.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gheyuzvgd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gnryakcqh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/grvvhjrqw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gajwyintc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gmzawyirm.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gbajqflsq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gwymvljbc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/ghphxiuap.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gsnpttdqb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gsukxkxtz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gpcwxhgmq.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gtpfwqyfv.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gdrnyjfod.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/glbizqben.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gnhyoftob.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gaydkznkt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gkjwqtzrr.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gtartnpwj.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gogtfltgs.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gxohukkij.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gnclfrzha.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gettfuyco.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gintnodzh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzzxexz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtpntycar.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gpyvllmfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/grawpjmeo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gflaibfqv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gfygawshu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gureprvsd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gnzhfzsnn.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyohatmvz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gvporltfk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gggidsoqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gtfxicldb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gladexxdv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gexgjgaes.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gogmtrhbp.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gqmujsorr.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gsxxcxhbr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsijrwmaa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gexlwamum.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gglhtjfwn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/ghcrqauod.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtkvpwhph.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gwrfiaiyw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/glcnpswtz.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gdgjfwbqm.sHtML


<!-- 参考信息 -->