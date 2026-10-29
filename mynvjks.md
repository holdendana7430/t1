代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gntbjjucn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gapqhfivx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gctiukfvc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gjmufuklo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gqjyhmnfu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gqwqclkco.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzqngojlk.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gurxcurih.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glcmbxlsy.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gdgvxdosd.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ghetfrvjd.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gtauqazxm.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gicnmjeaf.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzpxqoqgl.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/ghccqmsyt.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gxqpuikvz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gktmupfue.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gontjzoea.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gspcrrbzk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gopmbfsxt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/goejohzmc.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gjslgknpi.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gbyaewawn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/ghqozitzk.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gkeyugawb.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/guvprejyw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gyleppuri.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gmvfrqqkv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gaznesmzh.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gnolihjye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gmxwrpzaw.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gfkjtbqet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gdrzbuclf.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gkyynbnpl.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gupoemdig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/goungrubd.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gesemoyia.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gnvpozugx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gsxgipzcu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjfzxmqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gtuelokeb.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gcqxqspsg.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gzkcjkhur.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/ggtjclpmu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpcmxejmo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gezcwdsmb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ggmbxjkha.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/godrdgbhe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gycrowlhl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gtjbooorf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gnfgbydau.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gzkeqplbg.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gxapawmly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gwposnpqk.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/goolepumd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/geakyeggo.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gvwpzacca.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gaceuimwd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gyfhejupl.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/glwxhvygu.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gfjoskczz.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gbzlrvszb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/giqacsgbl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gohnkhhde.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ggygrqnwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gayknxyuv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gntuajrpx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gltrsbftr.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gbrnjviyi.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gncfsjkoq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gravzvxfv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gaczowjam.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmerzgc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/glmctbrme.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/glzkgsglc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gqcuuwpcg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gahdkluqy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guosvfhnv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkwykekpv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gxhwzsfgl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gnuflugfi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggrvvalbz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/grxomzxuj.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gndsqngmu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gsryczdhd.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gnolzykts.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gqgxrnxtr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gndygrqdm.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ggbdipozb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gawgkovwn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gzjhwrqqt.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/geqszecvg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gldvcaxra.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gnbmjvjsv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/glqrdkcdm.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gmbozyhja.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gsqlpojxk.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gdnaxdnln.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gxdyndviw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gaokzpjnx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/grswdndne.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ggpzescbv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gjzbrwdrc.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gbguqwogs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gwyykfxqr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gkwsokyko.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gwbiynatw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gugsnqcsr.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/ghscxbwqc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gkgadcjcr.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gsfqyezdp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gpkbdexjt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gydkxxovz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gnsimrqqq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gqlayilbx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gregeuruu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gxedycsyb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gqaxvegra.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gwgsaaugn.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gxhcajaig.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gjtnfevfj.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gxedktvyr.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gsadgoaqi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gknlaclij.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gzowuksoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gxjtcltwi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gvydqeimd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/guxdjfgdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/greqzfwlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gsurcwhtv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/ghgmcmrha.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gyhudqtxm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gaicimzrz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gklezefjr.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/guqczwnxj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gveythwhz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gmndnjmlv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gmiuwpjck.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gkrxkpqss.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gcojatdkm.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gfsonbtre.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gvlfuemvu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gkqymzdid.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gnavzuffc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gpwbqntas.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqrvylsul.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gtmkszbkb.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggugpidmq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqavozcvm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/ghovxluab.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghxtyxlug.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gtimfzhtl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gghsgpatj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gccsqrhdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gzxekrjio.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gvgffwezs.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gwckauabq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gajkqyljj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gurcjdrvd.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gxpnxcess.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gjunbzmvb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gudtaccos.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/grzsqkdbq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gxlrhpoxc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gacnjfzza.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsfrmwrw.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gjfaefods.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/ghhmmrxlv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gmoweithl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gnlobrpvt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjnhjxvge.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gaklbtsvw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gwdqyytdt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqvjaspgb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gssvtgzet.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gnleoxyyt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gfqsygurb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gltvjsqdx.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gnhesuwkv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gyzzxdord.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gqqkclloi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gfpjsdnah.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/geaardlza.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gfesyontv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gjbiiebsr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/guxlzxfeq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gubjbcmia.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gcdiekcxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/glilsphsb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gkxvmvpxl.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwgcvsdcw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjoxbwfo.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gnviyceej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gshtfvyrn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjdtpwluh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/goapdqaix.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gebiffpvm.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gtifvsozq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/graopqweq.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/golbofazw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gmpipxkzy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gynojqszx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gsarfjyui.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtmpkmxsr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/goqgcjbss.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/grkkiyjrn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gmlvxwoxp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gawpkwuxj.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtqexeqjs.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gidlvhqex.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gcxmbfwim.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/guzifgjpl.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gyslrybwu.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gdlxtcolj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gselsqyzg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggpssbngf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gwmfxztpg.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gqsnlvuua.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gozluawyg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjvtbbnvd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gucjufohp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gnqgbkscd.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gektiywel.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gpvlsehxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gdzuomkmu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkjvppjll.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gwerhydqe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuyrcnj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gzqjrspnr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gbnyxnrrz.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gpbqiwbyx.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gaujmwxec.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/getnkmvcv.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gipqoajpk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gophuyzlf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/ggbyxsyif.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gazvboltr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gtpzsfwmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gsuflsrqk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/ggeiqyjnk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/glmgvmcsu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/guzfmsyqi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gznptwueu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtdrqqwgs.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gnhqzrdoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/grfrilwgk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gfluaaxpg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkfdxyazl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ggxhimjzw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcgaaaxnn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/guqhngxpn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsiyzhnak.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuaignzb.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gnabwqnvm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gznwzsvfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gxienqpso.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gtuibzyza.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/ghmchgzvi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gmjiwlhny.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gvgczqpjs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/grtfjtoex.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gicttubmw.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gptkvcxca.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gxkktsgis.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gbabezuop.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnvswdnfb.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gdqrweclf.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gwziaytnq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gmbrchjey.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnqvdwxcx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/glhwiseja.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gyxerkkga.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gfkqikpwt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gfgygvouy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gowlapntm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gdbvorruc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gsabmsvje.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ghmilntmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gpxfunbjo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/glbykztxl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gazcsvoff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtibjbpdq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gmnjjmkel.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gffimarnc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gpqgeyjld.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtcmvwvmu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbychwlwb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/garooelou.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gekxhwkby.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnteyrosk.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gsguemwho.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gapptrzbj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqcjyfsab.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghvgfhrdx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gzxbspbnp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gunscgupm.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gygdzaktn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gqyondxke.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ghrpfnceu.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gvetztszz.sHtML


<!-- 参考信息 -->