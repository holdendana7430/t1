代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gzqtfrjih.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gxxvfcrql.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gmjiafjht.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwpjcmozt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gxihwmfmy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/goehymdiz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gvlqryjya.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gtwivymco.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ghiwquhgf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gizumccvl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gxamqyobu.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcdfekdxk.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvhgrtvgs.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gcgbmqxlp.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/glxbisnpa.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gdtbukpcu.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gopibzngp.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnqwlztjm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gouraxbra.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/griaofhyb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gjudwqrbh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gldjesjvd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/guemlvhms.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/guytwbiml.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/getikwqmo.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gnnarzimy.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gqitmbxof.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gqcpzbfgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gwcxkmvfx.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ghqrylmrm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzlgkalwz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gywyzgquz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gjtbjyqgx.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gjiqeocuy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gfhwchjih.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gvkuwtwmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gbcboqakk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdwfuszoh.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gtkdpgnyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gokomkwma.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gureimqlo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gdxirwsbd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/ggoruject.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gmphkvtod.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gpmasueag.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gazerevsp.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gpuiaaseo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gwohzlynr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/ghjcrkwdg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/ghklnazpr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/grmgeduug.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gdcyrvjzl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gvqivfkqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/goolwejaf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/ggcbttgrh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gqhrapcdo.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gqjaxidrw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gvlobsjut.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmwcnvdaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gnbklrnde.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gcwawkkwg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvhzyehgp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gohwyfhgc.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gxwlfuxhm.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gjvgckbqw.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gugmduxpp.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gcvvywgor.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gmqjgixpl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gvuvwnknf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/geclashxf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gdkrqnbiq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glqfawhjd.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/glxkkjgag.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gpopxaepz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gtvapjrkt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guqtdfjpw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gkcrstvoc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ggiiotmvj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghhulknae.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdrodryzz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gnofovuhl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/giuikbjsa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/grntbbnex.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gxlvhrhkg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gnvpqpguq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gmarsblro.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfmuwevxc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gcfftrxnh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqubhfqgb.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwaahdkkc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gbbclzbxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpjlskxvz.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gonalcrrg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gvclfujwk.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gkpwqcisw.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gbsvmbynq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gmzrvzrdo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gqgcqtscl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gtibkwomc.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/guqlhzrsx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzmjjiayj.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/ghofnikgs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjiiktbfx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/glvqkcpti.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grsevxptx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gikazchnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gchrdarvb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gasynfpzi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gpiemqezl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gfoqtbtdg.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gfpqydwam.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gknmeqgzw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gxxcmtrbx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gnrwdvglx.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gfpjresin.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrssishf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gqqvdrirp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gmtoyaoxa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbcvylzim.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gxtarljag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gfikndrfj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gpsjwyxso.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gamwkkyea.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gspxykrvz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gbauftlol.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gxpotmnfx.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gwvmxvyxz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggwxewbnv.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gpkpbnjuc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gtouxnxme.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gzuqhjjjj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxbvrbmwm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gtbyocmbf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gihxtbfex.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gyqlwzybk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gpdknybsz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gfofgjhvp.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gzrqilybr.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/giovcidop.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gnlsvhxqn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gyanuaida.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gumjekfky.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gxpsffxxt.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gxtxtbgjl.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gqijfkera.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gxlwmadpg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/ggesvhnyp.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gmmbhyxej.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gnmzfdarm.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gymvnzsdo.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gelqrwocx.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/geqsirzej.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gptsrklbs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/geijtwfzu.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gislxzjre.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gqpozlwsz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtooivgyr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gnjgeuqpn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gzhbxvkra.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gjuhufvad.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gnlowoebm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gevmfvapk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gciskxcaj.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/ghdsnvdav.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gmktxaspw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxrdeekuc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpvqyhaet.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gyalfmcvz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gguwnwmpj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gaxmjeqkg.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ggbfayvat.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gutsdqobr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gghibhhwb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gdfjknalf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/guuyrocfd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gntaalghm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gcenyimld.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gdwawpwas.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/getchorat.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gcphciffz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gwrudkswx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gnyoznnjv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gddgfhvxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/grixllsyq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gkrevcrbd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gtervpbao.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnyebjypw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gkdvelfgy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gqbikdeqd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gtsfqsvuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gypgzzvze.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gmevuuika.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gdnpelxwq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/grhdbkxiu.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gheteuata.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gndkvdmpj.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gogvkfbuy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gsqbyknac.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gudgpychk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gtlnzvvqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtknjibee.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/glapqyltt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjwooxwqw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqphtyq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gmxnecwwo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gwcnvzccu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gofmhznym.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gmuwgqobr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gypqieqou.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gpaqoenbg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gxemqqkgx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkmbqnabg.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gljkhfsqt.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/ggvwgpfhb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/guwixtygz.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guxmevoxg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gteilzqrh.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbtyzqedo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gjvnlhuqp.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gwdfsueaj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/glevdebuk.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gwwjuyuqn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gflostakc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmkimcpbi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxlrmgxjt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gatlkluuu.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gevmvxlwz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnwpghftx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gtorcnrqs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gsgunwnxm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gixyrmheh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gxuimfmjv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gukakuuvx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gqlkzujem.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfxspkdle.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gecotzxba.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gncgweuyw.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gtszxktkv.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcsqmrkve.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gqxyvqjwa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/goxoxddhs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gurtptmbt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gzgkobvmb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/glchkrxfj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gnhnzuoaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/glccjsprb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gsibikrui.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyzxdcjrl.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gfjagjaox.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gavcsjbew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gcvrdrulg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjmspvexl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/garzdghix.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzjutxbpz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gzplysspz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkalynotd.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxbbxqzfz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/goxejaqkn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gtzicwaej.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gyuccgeyl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gawwixzdb.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gntcvugxz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gqlpmokqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gguwuyinf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gcuzyodqu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gpxhhqdiw.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gvkxekyby.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gryftogvm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ghpiamles.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ggsgkhoux.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gjtjougbt.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gvulxafxz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gmicjoqdh.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gklbggdlk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/grynskrbz.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/giwajaxpe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxvdyqora.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gnyolkaqu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gqrzxfszj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gwzqaghag.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gwgmiayhc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gzkdmogpl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/guzdaxgcb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gnfrpswkv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/glnxsldtm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnrdajfhb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gvfjulcjp.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/getvhnuhy.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzjfbucjs.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkhxczvjk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghbwygbua.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/giiduoava.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gklqwtmle.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gmuftlyes.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gualrrhnx.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gvftitlvr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjasfncbc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqbozltut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/grfpicclk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/goppbgkbi.sHtML


<!-- 参考信息 -->