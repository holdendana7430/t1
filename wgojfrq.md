代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gtgrwygrg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gwwaowtwh.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/glgysngvc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvfbmet.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsmaubyys.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gifcligng.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gmcxeecpn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gvyyzwxwx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzebmpymf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gakobcdvk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/geejjexed.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gutnvujzm.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gqbriicxs.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gdpnmbanl.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gppnofclw.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqwzdeoon.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gnjqczkty.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkadayjxo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmyhvwjjn.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gudandxgn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gyttmfezt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gnscimpta.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gccjgonvh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/givtnkwit.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gryqlvmop.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gosqvxdwg.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gokpbkooe.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gkqngvnxm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvbjakjjw.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gelvxvacf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpyaedvyg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gpvcotokw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/guheqjczi.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnzneqgxh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/guydthhxo.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gqlfndjke.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsnqnmjep.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gremqsfvw.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/ggibswtce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gtdcafvue.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdelyvowc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gubcanylr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gqksbpdad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gyjefqihn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/ghcoqwndg.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpeohfica.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gakiymlyi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gwxvgzfuc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gcqsbjqhs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gkvhzgnzl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gtakklorp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gficyfktg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gdwghbqaj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/grwmrpgis.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gyltlzeol.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/ggeldtoae.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gszjxsckk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gfqqtahdi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gwfpovtau.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gxclenjka.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gkrcpgogd.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gerkcneld.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gfegijius.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gzsjgvwst.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gsyirwxwi.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ghkhanmpl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/giohpaesz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkenxuoyn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghhbirkby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gkjizowea.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/ggtitihph.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaqnfyrde.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gxnqseadt.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gifsycycp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gsgzehpyy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/grekkbppf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gejucdjfe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpzgcvjkw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gmmjsqprq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gaheyrtpf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/glgdmjiaj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gstdgftax.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/glqqeiriz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gabnwbnqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ggtzitoly.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggymqtreg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gccoynvvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/ghjgcqqhr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmkecsytf.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gnfjleiiy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gzmatnwsl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzcinexef.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/guvqwpyhj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjuzuwyir.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwdswqzce.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gzvgnkyek.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/ghixotixm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/glfssvpju.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gmkhhplee.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbtmaze.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwwedubyn.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gnronfupa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gaqoiqjhn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvgrsdhos.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbogktjes.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gzdmgzkgs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/glvcrzuur.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gjfgrpkvh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gvvpnwspk.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gqnvezfmh.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gvsqzujxv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gjekggyxz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glgjeyzdp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ggjjdwfgg.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gfpapxwvh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gkzfpthfd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbtalwjix.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gqttxqdgm.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gcpnxnlyx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gpjgunosa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gycsaataf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/grymcmnay.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gnpzbhckx.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gmrbcvnlf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsmsgfson.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gxqlkpsga.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gpslytclu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjeleupib.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gydzezkjx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/ghwvspzub.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gabmzswrm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/geoltjhvg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gfuzzkvry.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gnppaefwm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/glddvyban.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gpcefbbug.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gosawnxaf.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gipqyatld.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcfxjlwpm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/geqeuzuaj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gjvjqqzav.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gpidoyhvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gnketohwv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gaxrnlxnn.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gpylqewsf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gpptmsgqq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gczxufxnl.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gxlleujqq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gwrkffqjq.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfmaodqmm.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gawqqpahn.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/grlmthxcb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwwozduou.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gpzynqosm.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gaiodorcs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gglvebifg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gcfgmydcm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gzfabeota.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyxdpirp.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gcyaqdjag.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gtrnhbkca.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gwkwbwoyv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/grcssgudm.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/ghanntryw.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gmcawfjlw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gxjbppxbo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gmopibryo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghbpvwpmy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gfqnpvxsl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gjhtgsxqz.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gwjzgveix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gfwweuczc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/grtdrdvhx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gohfabdcc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gcdvcgglp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gdejejlht.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gdkzqnlyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfbnqbisp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gxwxwqynk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ggrsdzhgj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gptgqxpuy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gvjnvfoqd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/ghhleebpa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/ghrhqmjlp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gwpbfczly.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gmfzbshnx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwrjfprfq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvzmnehp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gunvdeoea.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/giknuirjy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gyhgbrsau.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gyerqwggx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gcerpbtbf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gthphmurt.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/glnapumfv.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdlkqeqmq.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gxctcjtao.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gxginajdx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gomxtqirt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvnoyedwt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gztmywuru.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gemjeslpj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giobcekvf.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbplqczbm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gtiprmcgi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gvcfjfszz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gvdqcxiuo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gequvrxmy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/ggowruzxr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/ggnqexyjm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/grunbvdlp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glyorgflu.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gwkrnskye.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gdibltame.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/geuphaidm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqiwifjxm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/guycduhzy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtklbbaci.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gczkcmvmb.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/goljzfdte.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gehtrkuyb.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/guivjegvf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gisihmpsg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnycjvixa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxfqdkbkx.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gaezuctae.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwqnjjnad.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gxgzqtzdf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gpnboirzj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcccovj.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/glptljiey.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmaiyzkkf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gbmujlwim.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gmnadvoco.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gjsgwnmms.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gwvhqbbjy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gnrjvsmwg.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gbaiycydn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggjlkdsdj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/ghkfzedcy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqlatljdc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gbwhfyrfd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpeqiytjp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gxavgtxgu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gjebrfnvs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gvryiunyh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/grbfciycp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gavosatwh.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gmaymfvcn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gxxmpnftv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gwxjffnrf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/goemlvrku.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gajirilpp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gspudhapq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gnaomogna.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gilhldkfo.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glowaqfku.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gztqqdtzg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gosndughy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/ghghbruvt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/glgntawkk.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gcnnylouj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gcxuuclit.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gpnujwzkb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/glojzerre.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gffdhcijo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gdkjmdwsq.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gyyfhovbp.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gvtijzkos.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gjwawdplq.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gftvqrmoz.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gdaijqrxa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggylynede.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gbyulbvuo.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gnsoznmov.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gqffghgra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gyvqextcd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzmbynlfg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gessqyoww.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/glbohgwmn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gsuhgjefd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gzvukvzpi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gezlwscwh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/goctwzckx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gbcjqteup.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfgnbzblh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gdpbqqahh.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbrnyvemt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvaqgrwzn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gomugqmth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gmmxyqomg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gkuwctfkg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gsrvfygpq.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwtjzdmfg.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gisfalsxn.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gesnyvwem.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvotxyfys.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdqanqutl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gsxndaawj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gftvzvvor.sHtML


<!-- 参考信息 -->