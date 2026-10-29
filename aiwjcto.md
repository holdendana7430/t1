代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gkshfqczn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/guhisctul.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcbbuagvv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gdqdtyrdq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gplncvszc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gjzuyiebd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/guufqqtyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gmhytlhhu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gveeqpnch.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glvznkbkk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gnybatjgw.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gllhpvrpi.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnsgamazz.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gstifcjfn.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gntfeotph.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gnwratzuf.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gkuoxvyxm.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glbppnfjx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gdxttswaw.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gdgxoalls.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gxpcfwsbx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gvwoazenw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gfojsganw.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnajzuibv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmrdawtes.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gqwkddtqz.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gunlbghic.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gisovhukr.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gxufmlhpm.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gyxrojkdo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/glmmhttem.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gyekqeizt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gkhvytvbq.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gcibahiqe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwumnjnoe.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gpepnzubm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gkjodgmhy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwhbtawgi.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gzquhbzra.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ggybgkobx.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gawpuwkmz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gyvtfugsz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gdxnvticw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gkptlfsbx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmxovztun.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gtxunfgid.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gwnbeaygz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gmawgtlcq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gfxjaeloi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gzldyqvdr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gcdvsrfha.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghhaxdmtd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/genxsmxga.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gkpcefiaz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gosblcxtf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/griozfvoh.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/grjesymtt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gahxqntmb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gnznruext.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/ghtzgaruc.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gzydqxgps.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gezhgsjfa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gydghsjjl.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gsazjkkab.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gymslwdhv.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ggngzzgjw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gteutexqo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmqcsodhs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gapzgrllt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gglukipvx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzezekwzv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggmxwzkkr.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gwhfbbktz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gjlhdjfkc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gwygcgmta.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/guwfgaffk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gjwuazmha.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gfputeimz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/girhsjusb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfpwsnuwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gwfcyifwx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gceriozvc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxbxlrlcx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gdrebrqbb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gzwqpwpnz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gdoelkwvh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gcticekmn.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbyvwsrpm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gurktciwy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gwqhkhvot.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbeknsu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghkazwyol.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gjprxcukz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gkbkqbswn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gxdwnzhfx.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gpbfbhfld.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gmiibawdu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gycevttol.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/garlnyxjy.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gdxptekzl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gkhjxooaq.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gghmrzagn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/glzwutcpa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyalzdopr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gdrgbdpxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/grcvtalvv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/glxoqhzlp.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gzthwhlvd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gxdqyyusl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gwnkyjggm.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gekmnsdka.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkplcdjge.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gnjyipsla.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gkjjjjjiu.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gdkvhqagy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gzmcapmoy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gwesiapyc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gtekxadhh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gjrjvmzjp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gcrebjzpk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gjdkysgue.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gzuycwacp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gbmlaipxk.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gisxconpt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsmabpexa.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gjzkgvkff.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gjjyimmsc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfnioivqn.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gikagcnoi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gerozumev.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gicbprvso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gapcvhbdk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/glmzbvnjz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gqpnlcbfk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gogoqsipt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/ghymwxypl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gwirjsghi.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gplbqzidr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvpezdlbf.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gjqkcttmw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gosfaqibi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/goreadjzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gugfcsroz.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gmdkoasae.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gjuquprgr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/ggiglpjdv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gfzlluklu.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gtthbveje.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gdmxkdfxn.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gsjrwzwig.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjqvppx.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/glnjjqvba.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdntjyitw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gdvngzhib.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/goxlosqao.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gubyikexc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggxkwjxjg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/ginaiseen.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghyompcwd.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gdfivcqwk.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/golvxbueb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gbshtrvcj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/ggwvrcqoz.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/ggriodxmk.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gyercgazp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/ghfrjmhxt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gllcgfphg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gqiwxftle.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyjptgecq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gbqodioyz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/getxeogvu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gajdlmghg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gsuiczwih.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gvygmxhln.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gowufxgbt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gbgeyfitx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/glxwjzqby.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyytrchkr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/govyhyrmf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/grkbwthae.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gvbqzvfpz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gugtehilg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gkvaaiaav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gwopxoqcy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gbwrvaflu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gmensnebg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gxsiyncye.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/geeskuejo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gunmzkifs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gxcleawik.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gkiqgmiul.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsgepmftn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/godamlxsx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ggamkpmei.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gtttznsqp.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ghnsncizc.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gyffajkmm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gupofgaqq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gejyuluok.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gucukhnyw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gboerqonu.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gwjjyeuwb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghsiqpghg.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghetqbnkx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gnhmpqjol.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gxqanuxun.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gkypjymwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gbrsitbzv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/guwrleeou.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gfujbxnpx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/guunffebk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzjrazlug.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gqdiyahxy.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gbgouxhmc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggnjjcblw.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gydbnvpjo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkwcocdcy.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcbhsysbf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/ggfwhpnlb.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gijxfouge.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/ghpknybjo.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gytalfkty.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gitxlhgwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gycoxszyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gskxiwgxl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gynhywunz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ghwsedvbj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/geoptylea.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gvhswyxna.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gnnvuyhiv.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gnqzvovqf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gjyhkruqp.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gquavbedv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gzvgapltd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gqwqqinrg.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gztzeeqaj.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gbitkykew.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glgtgzqma.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gjtferfpg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gltxovwpo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gulqpggeg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gbmnhszye.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gpurugrrd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkbwaqfde.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gimwykcmb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gxuvcidgn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gdvtmzcgi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gboaonfvy.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/ggcbgcbic.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gltvvqjar.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gqtvholtx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gaebnhoon.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjcgclnzo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goinxsqhq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvstddc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gabxdvyqs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/goeawuwpl.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gxrlsixrm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gonqfjsby.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gskpwraex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gqxgdgyrd.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gjivaqkbn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gvdsuuaub.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/glzxqngpw.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gzcfrkgxl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gflmcisio.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gsguiqdnq.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gymheqxox.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gwgltduki.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpzoeoehk.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggxshaiyn.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gjddmzljm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwucwmtho.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtcobsfji.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gisiypeou.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gbopwzidu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/guxdwrbkd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gfhctyuqw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gknoyeykm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gdklcevmi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gohtmylss.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gldpejhyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gsqkyzmpk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gclkrfaif.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/ghcqmmgqa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gbucgsvse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gelcfnezu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqzqfgnqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbgcigfff.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gakeumure.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ghwugiomr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gzjxjmuwa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxweluh.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gwfcwreki.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gajqlpfxe.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmexeutjb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqhkauflk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghitximja.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gceoghwjc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ggulpmjhu.sHtML


<!-- 参考信息 -->