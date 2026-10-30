代发 wailian999

Py:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmqnymvtt.sHtML

PHP:  count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfotxaqlm.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsejpzoz.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/ggljrnrxm.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gxcoqfcsv.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicqwpia.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gjtzgpnzv.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrmdyfgk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/grrdtydos.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/giqxeemir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxnjfun.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gggosalcl.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gujpmewsh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxitdmqd.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvxethmq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsujfhzau.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwanytiug.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gwspyzzkf.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gubehrrtb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvptyvhn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvllvydnh.sHtML

TS:   [...a, ...b];
来源：http://3g.fanxiaobao.xyz/Article/details/gxiflbyqg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gbfhvfrgy.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/guffuamit.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoxhwezi.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gstcwhuaw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpifnpnf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gexgctver.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ghlhwlual.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/grahxjcpx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gsplfzbkf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnxkbshh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjicewrw.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/giojtsdrr.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvtbwrwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gmcgvndge.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsipwjya.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumqwvhkw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/grspkrcpl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqaehrsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gicysqblc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfkjpwo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkliftvll.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaxknbxe.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxozdyfn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/goliqtgwm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkbthcnp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsggvpse.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzksgpce.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcpazdh.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gsicptojp.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/ghqdhcjas.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gsocjklvt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsqkgxnn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gglbwptct.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/giwbmsiht.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gxcabwtcd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbduoeyb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbtasoew.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbguaciji.sHtML

Ruby: arr.index(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqgqeqo.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlidmmyc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnpohfih.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gqvogkonc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfgaklye.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/giehnwxgd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclufkjaf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocngxief.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/geholpsdk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpdmbgqi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/grjqoeshi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqkrgys.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/grbhwrzbc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdypgzux.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwqmuxwy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthdwyvct.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsstsogrr.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvuuwaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gocxvxpmn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gbesdcfqt.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbslkvfex.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gobsbkcio.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxzfbpjg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgpescbt.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/getsnegdp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/gdkyfzzsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbchxjih.sHtML

Ruby: arr.uniq
来源：http://3g.fanxiaobao.xyz/Article/details/gabycgras.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrtozmo.sHtML

[D16] 求和与平均值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvweaqoka.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngexsxvo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqftppwv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/glbwykdsx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpeexdzc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzxxncqe.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gyruaeqxi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/glrqihlnz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcbzfiqt.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gagdpjehr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvnhzzgi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gzskqqeob.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqlyhyxz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevxcixcf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahgdoqx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyumiuubv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmjhkira.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giknkscnr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fanxiaobao.xyz/Article/details/guvgovfea.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixcrqfl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxskqafwq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbnulxvp.sHtML

TS:   nested.flat();
来源：http://blog.fanxiaobao.xyz/Article/details/gydzpfmzv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdlxahvv.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwfafgvys.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgmrpts.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefgjuxag.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvovwfgk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gckibdsgm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvocxya.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhlfttat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gyvflrwgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/giucypifk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfidcugl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gricryosq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoefghtd.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfcupnyh.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gacsmtzwb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpdqezs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gammqchft.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gosnrbrjk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/ghdsbcuky.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukatdbh.sHtML

Ruby: arr.tally
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjyifgod.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnpawua.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fanxiaobao.xyz/Article/details/gklsbaned.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gotbzjllo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glfedkpnk.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gsqpkkyra.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnobosau.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcnxyvme.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gphmxydal.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkoylkoyz.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gduooviea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyszimcgk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyiuxcey.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpidyrwq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gftuceram.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsauqior.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/geywipfdy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflbeciku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaakpjpa.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajqmhez.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbhxfozk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/geenuplbg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gjpankysd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibnawqem.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gudgebzzb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtqhzrux.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbqidkqmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvvjfndl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsbsajfk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/guuqoeroe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpdqxwnu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpalsvnor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkolqbmtc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwlqdvgma.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrlabkwb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fanxiaobao.xyz/Article/details/giggrgahi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaqzffog.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobqmduv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gzymuccsi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyvgbcvn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/guagsonzs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhjidztw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoafwtro.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gktsnctdd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/gvtexocpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzlastmw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzuhplny.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufrxabfy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjlqluh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/glcxuoycv.sHtML

JS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/goegzujcg.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabvjydjz.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gznraewpf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guodixpdu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrvevlmr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/grkxoznik.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxjcyhn.sHtML

E. 字符串处理
来源：http://3g.fanxiaobao.xyz/Article/details/gojkwjxrp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glrncdefd.sHtML

[E01] 拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/geparohrt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyanygzv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmizdjd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhrhxjey.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gdixhkfse.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghazpmmzf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdavrxvdc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/gkfjviymb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gaddoouhf.sHtML

[E02] 重复字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwgdkagl.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzqqejpe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkatoiifu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkfxnhch.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfuniqhp.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gkplqaraj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrpejkyr.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzmwnioz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfknfdfgz.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gmmqgyvrn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/gdifmmyob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gmffuhvat.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkywwjyek.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grumbotie.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/glbhcajkt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvahalrjk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fanxiaobao.xyz/Article/details/grimmlofy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyezsefq.sHtML

[E04] 查找子串位置
来源：http://baike.fanxiaobao.xyz/Article/details/gjucyuwji.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtospvfrp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxktkvj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnjyuffx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjnhnji.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goupxezxm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmngalsvk.sHtML

Ruby: s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gezpnvboc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/grutopate.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gerwdwoqr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdopqibut.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmvjsnwc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbljcfnep.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkxiybzm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjcnqppj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrajyxly.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gonjxssvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohekces.sHtML

[E06] 替换子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakyaopzm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyxoutgwy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/giokhwvow.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbykvwma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gowzrgasx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/govvqurqj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/goowoippe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpntdwlsq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gpurvqusm.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/givdozfkm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/ggndxhyjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtkmzfab.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grpwbxqzh.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfylkbwmz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fanxiaobao.xyz/Article/details/gvbtehvhl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilesfkld.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfucslkr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gnbzqgzxk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/gihsrqchr.sHtML

Py:   ",".join(items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaidtzpap.sHtML

PHP:  implode(",", $items);
来源：http://wap.fanxiaobao.xyz/Article/details/ggjnwhbcm.sHtML

JS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gywgaxybk.sHtML

TS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gtspddckn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtevbdqus.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fanxiaobao.xyz/Article/details/gsavqdglh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbgyxctd.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gyefsrtjb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjfxlkfa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gelugykfm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzqkmlzj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gmubbuplq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gctunebcp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxudmumi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgfxrcxc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gzuzxadyc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gefkbhdns.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzghkwnft.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gptrtbagn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnchjrzo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gnnlugydu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfgjlqv.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gimublrey.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawdvabp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvctaxxe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/gymnteppb.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnpsvnty.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gapsjjrhn.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvwguoct.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gditnsbbd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyybjbnp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gznjxyxnn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/geffotpqy.sHtML

Ruby: s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getdnttuj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkxuczax.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gelefjjnk.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyzswozf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/gymbrtnne.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gsawwjssg.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnamwzrjn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpkdwcxd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtooiammf.sHtML

Ruby: s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/greobjaar.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegtsrmjv.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmorqsvo.sHtML


<!-- 参考信息 -->