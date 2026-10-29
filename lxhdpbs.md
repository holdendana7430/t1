代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/guywquuxm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gtikxxyfe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/grvzesety.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gxoinuqiw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gzneltdgd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfnahnwwg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtbzpfwoz.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/giiqnmtgc.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gatoehhmc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gplaqgoxa.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gqhkmhmfp.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ghcpvqiqb.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ghxggvspy.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grwlrzpga.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gckxopzhu.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gfijzxfwt.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gwfikyera.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gyliiqdxq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gxbadzjwn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gqtsdjwax.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gblltrija.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gobkvseab.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gcpkwpbss.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gnghrcjvn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gsfphdfaa.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gpsgvnien.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/ggnezmyvw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gfiabmcvv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gwocofrim.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/grpzxffea.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gybuucamx.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gefwzxqbf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxhashc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkaztwbxs.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gjrbjrhnx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gzpwppuai.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gzsglgsza.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gkxeitmpi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gfozwztrh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gpmdzpiol.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/grdlcaait.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ghqfpuwcb.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/ggkkdjjyn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gssjqtdiq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gmdiciwvt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gadxlnsjs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/grdpbchsh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/ggqwqwuie.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gkchxskej.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gtpjsewnn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gdancbtcr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/growztaya.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gyzgkjgow.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/guvpsegsb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/guckqiusq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/godghxupn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/ghhzgnhqp.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/geztbifff.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gawwbfobv.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gdqixwrvu.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gpqzoirwq.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gptbhhpxt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gxldjitnd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbgyxljwb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/geotnwqqf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gygbhocvc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/goqonmkfn.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/garnfctdw.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gtetdsbhw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gyaebaqet.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gnvjltvhl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gsfbcefcb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gnvgmcknn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdensstrf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbpgmuucy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwmrwwbcj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gzmbemayk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gxmnvnbsc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzvqepwkk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqcyjpk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghqtumvkm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/grgjdsvmz.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gmduirzlu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gdqlsfsst.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gcndlezmd.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gjyquchnb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gqlurpuvp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzhcszhnh.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gvwddjhpi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gbshygrpz.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gvohyzbuv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gshtcbgcu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/grxxksncl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gqldgekfr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gniusprdj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gzldzwffv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gjctgtblg.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gaezcnsvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gpslqopww.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwbaejymk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcvnipqis.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggvorbdmg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/guheczffi.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/guyoxklfx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gpkcldgox.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/grgqlunci.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gqkelxuyj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbxntgxdn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gdvnwxdso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtbfsqmge.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxbsnjboh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gadaicfai.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuulbmpp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gtgqeotto.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gucssoypj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/grhdzwhts.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/galrhitmw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gecffnwoo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/goaudtiru.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/grqaeoxdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gtljsuwbm.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gzqedenjm.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gvjvxccmr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvvgyccwl.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gykhoezad.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkkrthdvh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gqpsryijw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/ghhgeyncu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gckqzdngy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/guliezbjw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gcoymnndb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gtqvnotfb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gumzbhaix.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gxplozdmw.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/ghmbdpzbf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxcypmhrk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gomewmrlj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gnudyikhc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gwqllcdan.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gddzayfpt.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gnvoswywi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/goanwopok.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/grihslwje.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/ghsprwvox.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gpgirsdmc.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gbgcvaqam.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gxefnlpju.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnyngdezx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghwuggqds.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/grsoxojye.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdjcjimdd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/ghphhtsdd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gedeimwom.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gixqlqedo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gyiqlhjxd.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gwfltvmtg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/giiyjmznd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gqjjdemvw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gniwpipop.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gmeyrsfth.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gvydwbjoy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkgxoaicw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkuimzfxw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnladqnkj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gibuljasm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gzlbrmpfh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/grvyukkzz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gmzffhilb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdqyuom.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gonqazkef.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gkzogplxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gntyevvih.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gksfpbnsn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gudwmcsur.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gnapftcte.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gtqcavthy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/glsicfyru.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gmyskdogc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gfrdnhpea.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gflyyobsm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gtjxvpwmx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gkgfjojbp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gztoylxoj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gmutnrkkl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gqabasfbv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gnijldtle.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gscpcbqsb.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqdamyyrp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gwfeoqzhp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/ggdhsetuk.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gswygoixw.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/geijhsvos.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghnwffujf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gwjkxtchv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gavzcrpqh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/govjovltt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gufxseuvn.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/ghggkyzyf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnxmcwwib.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gmfzzshbk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gewybvcwf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gmapbdngv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gascgjiqz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/goknqxzpg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gijjlmkzh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gnyvebwdw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gjjwiybac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggbehqxfb.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gifuutoiz.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gounfvdmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gfrcxlhpf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gpeqrdagb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gxovgcpog.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gukceucsx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtelxqcij.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gptaqjmeo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gbbjuatrh.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gtwknupik.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gtgutcivk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmphvasvr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcqpvjtk.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gyemzqwtp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gavlfkuek.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gwjjaeweq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/ggzkzdoxj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gcijzpkhj.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/ghntlccwb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gjdbkbhih.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gbmzzecvq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gwkegkrwa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gvyuqozli.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/glblrucmi.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/ghbhajeaa.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gjdbzgemj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gioohzxkd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gmcbqybpk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gttjlglhn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gzbylbdya.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbwzqjyc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gxkkkwcve.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gwdgcxymw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gemhcunpn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gnnowzusq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/ghqlqgzhr.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gjthuptdl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghmoauoht.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ggmccdelc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grmsmmlbm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gstesozbg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfxjipztp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gvjuqqluu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjgriklul.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtonffse.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/glnbextsb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gipqklynd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghffzyidc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gmwkkywak.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gkcbyfrsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/grtykbpdy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/grfxchtoy.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gogglqeju.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gbgrpbzed.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/geidgcifh.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/ghugxcyjf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gxvvbyzwi.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/giswofziu.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gizsbnzmh.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gihtmjqah.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/goefodpmj.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gsfqpmuns.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gcgftbjgn.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdbshxtge.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gxhlozrqi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvnbgvvkf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggehvvqki.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gfdpexadv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gqhuyiwfx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gklqjmywi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gtcuuralu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gdlmxyxcr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gyyviohgr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzsadeppz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gyptvgzdc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdobvgdth.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/giddbfpzf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gthbbcdkl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gmfustbhh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/grreeulch.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gjblxepyg.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gbsgubnlg.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/ghigmpipn.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gghemmucx.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcaaxmoja.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcsgxelvl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmjcqmpva.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/ggbcdqais.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gtjtsnwhm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfvfmentv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvybcznst.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gisftrync.sHtML


<!-- 参考信息 -->