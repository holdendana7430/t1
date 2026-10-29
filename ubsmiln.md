代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghjlqvbfl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gucnfwoxw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gxnptzyxf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/grvytudog.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtjldsjou.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gpmruzqgr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gdbvbtymd.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyrptmrxi.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gulivzdpp.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxydzisbk.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gexvojunb.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gtqwacztx.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gexldzlhx.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gliudciaw.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/ghsszqoqf.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/glzvixxvs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gyudkgphm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gthkkitvy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/guqkavsmn.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtfbfyfle.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtnnvhlds.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gizyzoajt.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gazgkejwg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/guqzqdjei.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gmbnqyqcp.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gmupmwwct.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gbgtarxia.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/guijpnztf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gugafreye.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gibtnfoko.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gncuqkund.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gzbywypea.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gmjkbgmro.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gapsffjnh.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gmwqfomwb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjqkyxmaj.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gudwywrrp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/grzdflwfh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gnvaynmll.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gcubideto.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gbofkzycr.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gaoqxdivb.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gumgpznrv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gafqdcpgv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gnelbiigw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gzqgbtihn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/glisswyvo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gukstvrll.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gqzghawak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gvsqzvzmx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gddyxrmyh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gimlprxln.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gqgnfkgbl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gauettkal.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtdteeur.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gjndezhxa.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gmflnyecj.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gkduecfxb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzgmpioqd.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/godpjjvic.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gelbwjzqw.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gyvghklpa.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/ggqidnnwm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqyxpdrvs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcsocjdxi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkkgkmyrz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/girnlcaag.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpnwiijdx.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gcxsvttmd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gufqgoljk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gbqbadlue.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gzsjfgfbp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gllyfmgou.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmzfloalu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjflojxin.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/goorymhqm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gupkhimxs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gyeruwgqh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gnwmjtkeo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gaqhhulqb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwebergbu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gockljxmv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmajmkxun.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkbqoabaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gnyuctviy.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gnwisytkh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqwsqybwk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmauzgjif.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gtugyabyj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfetetbah.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gfzfbbsrx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gfmeqmlcq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzdqtshrk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gixwcehpi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/guvzbiglz.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gxctjybbo.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gmvtnzzto.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gxpkuhknv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfbokzfbk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guchdhoyg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzvhsusoj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gutisazjg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gomsdgbac.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gpdpbwuwh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gmtcqbqdl.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gjjomqclm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgtmvsx.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/guxixktgs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnxuwctse.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gzpcvaksm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gowooyrux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gircexves.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gbhthrrus.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gioovatgx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gvhffgyzt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gximbkdwm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gilzhihfw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gqztiihxk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gzwzwumzp.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gjjmnyfgb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gcuduqvuv.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gbzukilyc.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gvleeyeqw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gujdmjjnr.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gdswxaxpv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gflwcqqrb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gmejpavel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gycrfaafp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gwbkrucjz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/glnxstkre.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/grbqqzgbj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gphcgdxcr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gbybyzkfo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gwqhjtwlh.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gewkeftlu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gfmdcxmvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvimapczu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqrplsddo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gndqiieqf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gnrjqzdfp.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/goecchevd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gsplfbikq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gtkbzhecu.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gcttajkpt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gzrexraka.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glpoxzgbb.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/glmmjmdlv.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gngqfmlys.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnygusgtw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gxnfkzeeo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkcvkaphh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/ggnwhslte.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gmgywyjdx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gmnjgpqxw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/grhnkvqlq.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gqxugyqlw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/glekjcftv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gxfywamyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gdztmwtkn.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/grqgfystx.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gdiwawroy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gidukgtqy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnsyslwyo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gkhezcniv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbbujjvns.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gujhypfym.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/giqxnmygx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gjounxzag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gclyhcppw.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gmttctxpi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gwcyvpucl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gviferrsa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gxpwzweil.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmwymmolj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gxzzmcxfq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gpwgapphs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gxkwwygnc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/glqrqmqjl.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gtagzmrqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gkbogrqhj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/giczawkpx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gpnvtbxni.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gitmvczht.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gffvenwul.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/goiidaxoi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gmxuxnvbu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gnwmieixw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gakrncyto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/grbufljtf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfmnampsb.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gztipspsp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gvmtqunrf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdsrtoxwt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gttxicghr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gpjteisro.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gthymdobr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggzoxrwxp.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gqqhpboyp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goxjrayin.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/galgatndp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gpxcbpzyi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gcbhfloii.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gxhanjkbq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gofzwyqlk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gogvaipxu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/giknjpjvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gvehphbck.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxkbihopx.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gxgwfmgpj.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/giecfbspk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gjemoeufu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ghgcanrue.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gxpdhcxut.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gdcuglyus.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gnnkajtbw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gydzjlvln.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/geevaxgew.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gptkfnihg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gumhjpuej.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gntjohvaf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gdiycuzlf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwnjylska.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gidlcpxfi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gkyroykvw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/galbobxoj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyegapthr.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gihwxilpd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gvbxzgncf.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gptbdsbrd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqtkzpk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gboazkkaq.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmpmtydvr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gxtmxabyy.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gvluqmtjn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gyndadvwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gbajgmkaw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/ghxqibnyw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gqcayszri.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/glzktoxju.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gsudazoeg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gvdzwzbfa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gsnnfqzih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gnnqgdsfk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gknhjoizg.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gkwqtnxop.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gohplnylg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gcpinnsjs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfbifautp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxbdgbodp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtyidvlgu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gfcvmrvwj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggkerpinu.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdpitzfws.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gtmwwhshp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gaxnmjgkg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/goteixcvc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/goyxqcsgf.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gfnvziwhl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gssrmeukg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gcevkracj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/ghvchwncp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gezxpccvj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gjqjvmhkx.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gdglvlvov.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzidyhzt.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdlhyesao.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/grtijfirr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmcrnkmjs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxfmelwf.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gydaienvv.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gcerllrpw.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gzztbpywk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gxxztvtsc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gjwswifai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxfkiqtvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/ghxvrtpny.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gihhpymok.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gmrvwuhsa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/grmkjgmxr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnjbmjyxx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gtpqhfnev.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqnpvqwbs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/ggywdxihi.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghifvffsl.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ghakfkbtj.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gprtbmuyb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnwpiyxjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzoljuebi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gzjdmraut.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gwcspyqdd.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/giuslgmpk.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gzqhrmblq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjhhzukfi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gbwqsyxsu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gnvhidmkc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/ggcgfrpjz.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwcgmxggi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gitmphfyo.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gadtkguau.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gsyynqpod.sHtML


<!-- 参考信息 -->