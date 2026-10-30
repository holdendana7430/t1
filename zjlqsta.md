代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gzvsrjybx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gwgmcymuq.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/glsduvbjy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gspyzrblk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxfyeuwky.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gkuqzqfzw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ggxdbqjrm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gpjjjlmyt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gcduxhspr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gnlnhoxsm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gkwymmfet.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gwxpxdmni.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/ghbnuietg.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gtkalhrlm.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gyvdnwwmw.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gafxbmfdo.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gmkuzoxuz.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzjloeu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gzqaeamay.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gvmafmhge.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gsgecfsur.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/ggietfoos.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gwppbihcb.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjwpexcky.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gufkyzdoo.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/guxsmjodm.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gxuagjnvq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gtohuauew.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/grnjszjnj.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/glkjxddle.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gpojkdtzq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gclltotsk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/glldcpanh.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gbpohroli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gstcmnohp.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gjfnpuczf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gwvbapnyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gtintpour.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gqpasbhhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwqwqeecz.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/glhkghcrb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gxigzauyj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gxixcrhjg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/geslmkkdy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxzceplkh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gtopkbdea.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/glrfhbrnf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/giynzrnwu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gjdxqbgnr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gkcqcsydv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gtnolnspv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gzpemlixs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gbxewpswy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gntbkidry.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gjbyqyhlz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gspoegfdd.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gkmsxpgyj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gchlyyapn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwyhdzxay.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gcmacazny.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gaxoqataa.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/ghudpbuxa.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gtlmynvtv.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gfmsldpns.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/grapcbotd.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gvwhalmou.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gfpbdidhq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbgletfwc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gbcqpndkg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gwmiaeubm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gmwtxcurc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqgmzqzys.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gmasfioeo.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gseypwdax.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/geykydzkf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gvsfbbpgs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gagufikpe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gatrvfonh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/glnxvufdu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gjhlfbsgv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gmxmbrljk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gbfzgbwey.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/grkncgqgz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gdhowuhhc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gdrtwoeya.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gogqymksk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gzuxuxjmz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gvdybzeot.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqmkidxne.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzsxhdoev.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmwtyuzau.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkugzxvgh.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gwhngzzfx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gahpvitdn.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gjjtszmix.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gmjsgxryq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnbjxkzpt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gxexlgpjk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gailqqdde.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gummelaiv.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gcijelpsy.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gzfuobupy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gbjyquvbx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtdrjxysa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ghhxqxoju.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gbvqtyosy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gbqxbgiay.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gqvrzdmsj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gsixnozde.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gugwhrrhi.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gjgbtrxfd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnogtjnkw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/glndgepxa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gylwewvju.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/giwqenhwk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghuqdgyit.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gseiabbmq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gpuifwozz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gmdjwewqv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gntcbkfdg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/geayuyjef.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/guktiniky.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gzsvnmcak.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gztvlzbxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/guuzkkvke.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/goqdxfxxl.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/glmmjgimz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/guevzgjew.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gqrswzulo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gopubxpor.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwfdnaugh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gzqbcdlox.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/glnleczbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gpsexsvgj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gwqqxfqvh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gowhzvzvo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gmwwpuxto.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/geztlvpth.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gteoqfpsq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gcejtnfmd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ghzvjzseo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/giuwykeqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gfkdxoovm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/goxothxws.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gqepxtwga.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gevlbbmwi.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gjstevaiy.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gymgyhegx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gxbjqqjbe.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/geaxdgqyy.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvgaobedj.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gusyfssaa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdazwtmxy.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gubcdtqwz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwyxnpggu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gcfduzsfv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gqnhlyxwq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gjxucxhpw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gdkzujvkg.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glkzlnrut.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gilujkpqs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmzhcvaxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/giebyipjb.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/ggmezugeu.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/glzcellgl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gtwufbygw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyyhnpjp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gzhdnrgey.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/glhkssosk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gecrlsaal.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gvnwgktyc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gncctcrqq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/grshirzqq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/giniitudl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gowxetgic.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gnnijiete.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gngjawhyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gytkjybor.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/guwseiecy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gzaaxrltc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/ghqejexoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gsmnzzmkn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gckacfjvc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gkxkxfsof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gytbeumoy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gkibxyvom.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gmcglkoem.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdvpilcsq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gsbhgrrym.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqymxyxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gdidehuja.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghnjidrsx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/ggxwzjvyu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gwyvkapnw.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gncowogzh.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gaoxcpxtv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/grllyayuc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gkrdqvtkd.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gocygdtbi.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/ghxeqndpy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpykqvybh.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gtaieczju.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzkivewfv.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzidasbjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gejlxtupt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gwrrrsfzq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghddmpgzs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gtjzeuhfe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gybfihjpc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gvdoocrjn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gjfvhppaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gemxvpczi.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gqfvaasbg.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gewylgngh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gsqkqxyrv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvninynok.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gstkmkvuu.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gmfdltrgx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gesnjrham.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gryzbaodj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gnzbmlkyg.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gtcwwiyjc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gtgbfhkzh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmfraorde.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvvnthbda.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ggjewjszm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ggnfhufvz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gdrasndqj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/guwjvlasl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqxrnedkr.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/geknrtept.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvruvdikb.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gnifcuiat.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/guwmnxkhn.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxopxhaem.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gydikgqqy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gwjfslbyb.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gamaybllc.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gehcqcpub.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/glrlbwgxs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gfznuvjin.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/ggvuybyrj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxagyfvaa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzvlmtxbv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gpjxupxbg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/giukzlckm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gxboubnxk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ghzedreet.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/geqcowgru.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkgkkyfqc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gzvtslfnh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqkvzlsfd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gafnmwxhp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggoddbnvj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gdzriuoye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gldafrezn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxfkwwcqw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gjfumdulm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gbjmkwnag.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gjczemefp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gafaenvin.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/geqxzodjo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gcksgwvwh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gphupfbph.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gjaifzzld.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gqofrfwxp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gfcbeiyqz.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/grtysdgwx.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gvarqvont.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwyovzfce.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gpjmhggwq.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gnecrmfeg.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gevmjgjli.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gkkklcekh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gtuncxvwl.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gjjatdlid.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gtgoyedhf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/ggxhzzcuw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzgqcomby.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gheldtqml.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gkernwwld.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gtsfitjhe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gsuvoxhqk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gzabiwqyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gaqnqvfqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gvkpjdeob.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gxxgzneay.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gguofbaci.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxmhpvyre.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/goyxdeyxt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbzdmegaf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gyazfjfgh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gthnzmqxk.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gxrzmvjap.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/guskwnnsp.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/glqkteeae.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzieixmzv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gutlhnujg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gytsidxmi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzxrtzl.sHtML


<!-- 参考信息 -->