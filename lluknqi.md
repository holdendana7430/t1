代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqoswgmdx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gipeggadg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjaueubvw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gzjfleujx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gelysnolo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gplzbcvpj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gehcyqxuq.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gsfpxqekm.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gizjqxacs.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcqeqoyty.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/glcohcclr.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gktgddhex.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gfgaburny.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzyzcyyei.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gntrezmrk.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gdigxmyxb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gbohbvbfu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gaatbmvcd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjrrbtdaa.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwgmryvzc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpyctjncu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gppmeqmrl.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gjgyfyxva.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gjqepicob.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gaiwvfqll.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gbrxbdqbp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gcjypwkyf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwrdkiluv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gnmdaeymq.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/glkkpioqd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gmqlxswmi.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbxnjzfp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/goyewzvhh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/grycsrtcf.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gvpjqbcdx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/guqtceutd.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gbhhzgeev.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/ggrxgbjqe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gamsfnidi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gmvxsogmg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gpfeeslxc.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gcmlsdylw.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gyetyifzj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ghgcasvgp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gssvzyzap.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbmxdxam.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grofkawcm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gicliedww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/guoccrjbj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gmndodede.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gzzccfqyp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gywbmndqp.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gynsbwjdn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gdufcfape.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gbhauoikw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gkaseufsi.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gzpwmftdc.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gqujkytbu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gahcagfgg.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gztwgfiuq.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gxyyodkld.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gvszsitjj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gutjynkzf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gowhqclak.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gmtlrymmu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gioswjmcp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gonogrxxq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gffzeideu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gpznzjrxt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/ghsyfghwh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gpuyebqti.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmxaimhtq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gzkvzocgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gcmyjktvw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gqafneman.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggxrtrbsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gfpfffytd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gzownujoz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnlrgbjvf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gsqmwjadx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/grvbdmvcm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/glqgeirpf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/giryveoyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/glrtzzufl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gmuzfmjmf.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gqlsmtnly.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gzjvszalm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggozoywsz.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gyhpvshyy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gwdpprzot.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gxqrvvxes.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnhdngjrs.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/glydbjpab.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gslfgxalw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gcroucolr.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/ghgcepess.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gylkbfutw.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gpmklzsua.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpqwatcms.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gplmmwmpj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gadwhdelm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghaswudma.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gvsbkmsul.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrmqvpp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gjrhgjmyl.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ghbukggqs.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtvehjocv.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/guubalrrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gynkacwjn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gkggnbsfk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gecshhewr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gfbbsqfvr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdrasqylt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gilbftgbr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gfgtvqctm.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gzvjlwhkd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gugvkocyq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gruwnfklr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/glgmdwgis.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gamdqcpda.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gkrzfzcay.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gttorzuuo.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gkubpiuoi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjiqwla.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gcccoajxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gbkouylge.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gtkrmcbsb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gqduewjjy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gshfjarbf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gnukuiafl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gwykvvppv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gtmpmvisn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/ggwlrgxfe.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/grzjftkiz.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/grgjhzwbf.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gkreethrq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gtxybjylu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gxmjmxrim.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/grjnerlkz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gynpwvqcc.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gkwsrzxjq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gouyqsyak.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gsvxslqum.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/grwmrcwqd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gwbizvayt.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gglngiobc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gscyqdntc.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gruktxxur.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcijuofnl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gbhijysqd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxdkjmrze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gegfusasv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/glbnsxyct.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ggtndjttl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gngdswoef.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gaedzauhs.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmywjrkxo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/guygvkscu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/grnpglkjt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gjqqtmysa.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gszhoufmp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/giiqifnkt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkhrznvbi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gerxrizwb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtthohoib.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gecoiutfy.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyagalafe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gwghohxcx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gmtaewyzm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gectrelib.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gdfnjnkml.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gaubgmzzc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gbivelsek.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkahnhrpn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gfwnrbwuw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/guyjzjqzh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gjkagoxey.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gepfzuyyo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gfedxyeox.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbebgnlyb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gbqazflej.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/grjewqcgp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gwhvuwbyq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gbgoxuzfr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gsggmgfph.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gzhyovtit.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gnmbhgqgu.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gotavknea.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gwqrwbxek.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gxpkpgduv.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/geddrumts.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gtmckwcik.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjbconhi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gfhgpagar.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gigivgwxm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gmlpsgxep.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guqcntbvp.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gichfnxal.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gijcvkylw.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gefrcqueo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gounxzbhb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gpzpkdgvr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gdsrqlndp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gbasilvrs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gjtvdjfsw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/grxkdyyvk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gtsbfiezf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkrrvrris.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gexejrssp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gpsnbcfmo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gzpyqofsn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gmfoeohan.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gjjzqdemd.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvotvubfw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gnphucycp.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gkpeiuvro.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gkkxseinp.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gtchyxxxe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gjnxapmqy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gtgykmtep.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gsmkfommf.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gxxfanktg.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/glcwejvlt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gkremlwpr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gotbzyuia.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gocarjaup.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gszmvilcs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gzawmvson.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gnvchrvms.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gcguhowmx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gxxerbnfi.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxzkoxpiy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gnjfwuesf.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/ggansioxw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxiietjv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gucjdzkfo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/giezqigpy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/goqstsxvm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gcomkrvps.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gwyaajvmi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/glndutqll.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/giwtogrdz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/ggehqmfbn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlhbdlh.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gcfflkrma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gjhqshvvn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gkkukapza.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwrvjrrna.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gctvphytm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gavehgble.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gnrbcmpmj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsbvcwdpm.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gousrjkft.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gbgzvqcwf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gcwrlplaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gcezhdujk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gonfexoft.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gsbxwnusf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/ggmfcaaaz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gzqtupwdm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/geypkkmeh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ghcjjkkzc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gjdstyrou.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gryywjbvr.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gchvfkocu.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gbnwpnhyl.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwikzkkrw.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gubuyprnp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gapacbqol.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gxxhobezh.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpsocytg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/guriacpkj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gvegltwew.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gdfoamjtf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gsegmxtdd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gcmshevkl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzfkwouea.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gxehrsowh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/grrgzzvci.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gardzuqzn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gphpzhpem.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/guwxfupxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gjnvfrvzx.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gibesgvof.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpscwnewb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxnkiyypc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/geastnwiv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gbcpzkamd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gfpzhnfxp.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ggwlimipk.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gduwgmfqf.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjfsqza.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxbovrrcz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gjajywjws.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gncacolpm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gugguensk.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gwprisoep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gvrmabtkd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gbyxerbyv.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gttvqkbnp.sHtML


<!-- 参考信息 -->