代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gkhxrbepi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gawseduhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/guniakqcx.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ggdnhvtoj.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkjxtxqzk.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gesxgxvmn.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ggkiqfexn.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gusbeejuv.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gzkfceteh.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grbccuimi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gqyxkyfje.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gcuqovqna.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/ggaztovfe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/grylwudmm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gcvfnfite.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjwlcgjch.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtlsiqbkp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbbxqkvcj.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gnhqoyjbb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gsuveuqpz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtifcrwbk.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gabqqasab.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gjrmvpcqe.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gljtlflax.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gbihasajk.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gcqkozksm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gfxkkqfuv.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ggajrrdbr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbrcuwp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjqoiphbw.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gptfnevfg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ggaadsdul.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gkohsygsr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/grmbcywgx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdidsor.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/ggjdoyqld.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/godakcxxx.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gjeduyjhh.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gkrcptouz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gheosdrgy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gfclbeyag.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gcucixaeq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gtcjircem.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gnskpwxpa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gajyjbohk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gubezxwto.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ggjrktccq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gkjuibxwd.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gdfshmtbq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/guzouoltd.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gbnhymiii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/guqggzjrx.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gvmbszklv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gpczblcug.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gpatzkwph.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gngxktpip.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/ggcklzfjw.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gbmeddbla.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/glikkijoo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gszebomrq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gyhxlxoub.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grlgowemq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gdbrxkhpg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkbjsvdoc.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gqybleknx.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gqvdgvhoz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gtiqznfvw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gotvqcyrd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gpbkeqmyd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gvknzmlss.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gshotlrue.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gszcgeihg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gxruyixhq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gxydzdkvi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gksgkvxdr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gdjpogkom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/guvzimsxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/griimtkdb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtaocjemn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/geotcsqnl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqlhxbs.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gxwrcwycx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbcgqxmki.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/ggcaouhdj.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ganzkpkrr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvhdacxmu.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gxlwyasbh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/geettxpma.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gyebktpry.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gxueiwmsx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/guiktaefl.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gnnkdhwhj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgzjlhc.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gsboeuztk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gjizlzqiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grkvuakkv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gtolneefi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gvzxnjnlx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gclgkebmu.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gytowhjfi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/glokntoxl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gibfjvqje.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gtymbwcuv.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gkbnlddqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gbjfqdwvu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gwyesxlan.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gvtfickub.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqsktxoba.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goslfntlb.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gcqcnnxfi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/ghhathaao.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gzagpolfd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gfyyaffgy.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gyzvkjvyu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gsyqtvxux.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gericptwu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvoijwatm.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/ggpnfohgs.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gnziypaxn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzfywhpaz.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gdaxjmxvw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gxzdmrrka.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gvrhwzrtl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfzzeskak.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gvcmyrwan.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gtvnscjar.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/geoberezy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gvblacdvz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gepjvvblt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gsbatcuam.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gxqkvyqwn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gxesjlgsb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gwmcqafiy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gwnrdptof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/grjlmxmkz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gvainrhzw.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gjftekexk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gaxrdazuf.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gatwkypss.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gzbbhhvde.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gavqctezx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmtvldjwl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gabkgzwhb.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gxsnttsij.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbtcochbh.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/guqwdstbm.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gljyvawzw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gcgossnri.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxeenmiyf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gpvdbzfxa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gidbjlsyk.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/grdvtscfg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gzlgpvzpy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/glmljlnhc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/grkajrehy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxqbtqgrg.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gunjrmbzy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/ghivdtlcu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gdgatjvff.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gajtjieta.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gkywqxrtd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gzdbiasnm.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/grklqfnyz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gvjqdmkwp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gpwulvrie.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/ghozaukyh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gijhawywg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/grzrgcaud.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhjdyyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggvwocidk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gmxvxewkr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/glxqjyzcf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/geloripgc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gxpakevei.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/guxejimys.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/glnulaguu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gbhmxwafb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/glbcwpjzs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gxiprqoxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/geuuqzati.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/grqysdbdf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gmvmdfrrn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gybjrmayr.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gwacvnkod.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gaoiottpf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gkahilscc.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gspnvblph.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gpqzukhgf.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gwehlslwq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gsykiyowi.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gcbktnmgs.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gjorptdef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdjqbrgvz.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gwjxnncbj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsyrihflb.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gesvyziyz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/grcoqimsr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gyfjpzvqk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gmgzsmogc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gbkouilnh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gdenwmhwf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gssskfcvd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ggwyuzpfo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/geqzaxnaq.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gxcwjghhi.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gnqpbmpkp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghwywzxtf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gfmxnaanr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gnfxmbvie.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gctpvoolf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/goimyfmza.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gzrgcomul.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gpqyogpaq.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gftqybbmu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gjnqxtzge.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmakaeras.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gehmlzvzl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gorhzsebm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gcpbhattc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gktmeimsz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gwtohzvam.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gcmtllmqh.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gbatfzpmo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/grcxwkatx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gallbqdcc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gcgolecej.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gdjdfnjjo.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gwejxfidh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/glzssayrj.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gcamvfeje.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxtrdzsda.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gwpoclpdv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/grzzxtiwm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gknvtqxhs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gpublekio.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gliaaksxi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmwdoaafa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/guvfgpdba.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/ggcephdaw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gmozsoqcn.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxtetnqlf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gpfaqaixe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnsoqcpk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbnhnomut.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ginmddqmt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpgsjjlqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/guprlnhri.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/ghvovgxwg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gttuehhjw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gybseichm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gqrzundqu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gizepisbx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gmbtrglet.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gbmkzfpkc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/grynavoit.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/glbfiulkc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gfyngakqv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/guyiuhvmm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gmzwhydos.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gbxvynkel.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ghhcozbfq.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/ghhygabsz.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gturbonjq.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ghrninbsk.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gmbvnytki.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gruxwhrfw.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gufsvcjkz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/ggqjuhiso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gynpxbdoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gdekzxmmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gwhaurszs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/grakmcdxk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmoaxvlaa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gqeqnskpj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gfpicfkkw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gxuiiirjc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gsadsiuli.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvkkomobu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gvggjjlbs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcsqsaibi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/guxxdggmv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwbpaulnx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnmedaity.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gsderxavc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gwimonvgg.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gcouvzaiw.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/geofqoayk.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gijxrcpxs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbnrbcwmp.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/glmbxmmte.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gsiqrkhek.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gvzacqcjz.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gkvcexuag.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gwgjdqlfc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gzgdtazib.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gwdhkqtzx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gkyogiczy.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/glyevivvt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gytxusvho.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gsthvdhin.sHtML


<!-- 参考信息 -->