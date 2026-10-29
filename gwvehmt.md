代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gvujzkxtp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gvropczxk.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gxexqlklo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gowkyfinx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ggupqmlxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gpehltbff.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/goygackxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gcunvznwm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gzgaketmj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gznxbzcun.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gnzlvhudl.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gskjninty.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcwftsyce.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkxwojgfl.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gajctsxtn.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gbryozuvo.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjorpxatb.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gcfjacxyv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gqixidvih.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gkewdaebu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/guhbmrzbc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gixaacade.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhxorcop.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqlpuxeha.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/glyryhqiv.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ggftazewk.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gspbukrug.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gvycdgykg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gezbkhscb.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gdgerxuok.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gjtycwdci.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gofevqllw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gmuqgejxy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gierepawz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gqlbkhuoh.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/geldudxnp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gjzuwqlbv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzrtacrej.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gqlfxhqob.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gqmgusjan.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gufdsmsrm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gsyyllnhy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gnsrhniks.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/glxaqrrzy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsaddkxyh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gboaebcrz.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gxiwxmczd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/guwzqxiup.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gywpopfqn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gsvztovmc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gbzouolrk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gyyytsnfz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvpevww.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gsscianqs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/getjxkeyx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gyjdaorkc.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gjeshbcqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gvjtjkocq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gvgxovzqi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/grqkbpeni.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gqcewwdgm.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gymcgktnr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gcvlqkmbo.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ggrktxomj.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gjdaoxzwc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gxhgscchi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdmdoqj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/glkvjzdvb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gzrkjzcgw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gbzrxgmkt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gmghfaxfl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfeobfiqb.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/ghwqvqnrr.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/glkusbrui.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gazwusewv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpuafafnz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/geiiircot.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gflaviorv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gwqgowdsm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gfmqlrkez.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/grpcbbuaa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/goghppmkk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gohmuydiw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/grshmkrrp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gpsbzhbpy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ggietawoh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gihmpeqqo.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ghumoklfv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/guddeexmc.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gsxqjipzs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gqrexzxmu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/giftxlayc.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/girrxrybc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gclsoemgj.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkrbanjgc.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gfbmrsqtn.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwiypwdhg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/grqpvhqbf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/ghtnbfvxy.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gbdpkxzhh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gflftbqly.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/guncuqowz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxfzabpoa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gpmiyxfeo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggacuykqv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gfcwyduml.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/geotyyswk.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/guvidxvmv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/ggtfkmtla.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gjmrrtjdc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gtpooyrja.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gtkshqwvt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/giorylpnt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gypwzgbcb.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gfjxupcyr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvjfufmqk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqhzxszfo.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gruafkgqm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gigwurmua.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gisbsxsvr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gobyztxsh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gedrzflnf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/ganqfesqb.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gtfmrduan.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gaoipxuxn.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gwpfbflch.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gvvydfrbm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gelbpvsgi.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gssvwleyn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gfxjrgiki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gpikvccsh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gjslsxlzs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/giaocokmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gmtdidioe.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gketetndq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gowyboupi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gaaijohpp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/geikocewv.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gskfvvkti.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gqobnfwpb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gbwnknrfy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/geuuiyrtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gpikwsqlp.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gxjusuzhe.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpcapzdkr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gpidzpmvi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/glvplmrrv.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gqvbzlvnq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gyzfpegfu.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvliabcbf.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/ghdqtbfll.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gwokycsze.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/garzarupl.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/ghsdygvwp.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gbiajizfy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gbokmasuq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gmlltxllv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gnsaxasfd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gdooimsst.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gxwahbioq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbzhxlatf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/guuhfoyrc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gwvtkxesw.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gjvtxnltv.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/grfotkyjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/ggqormwye.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gikymgcgl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gwjvctarb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwfahmvqq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gdwyjtlwh.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gvoooauuy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/guldkwypg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/ghhwlglnb.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gvqbrrnfi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gsnfrpduy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gsnzbghlf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gkbssmcij.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxbugktjb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gonqfofve.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gnxkvjetu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gkqgddiwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gnmezdvkc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gxlharczz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gjvxsxapk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/givponfch.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gzjvfqxij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gvnaypmyu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/ghlwpqgvq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gnojmtezh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gxdhyomcq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gpwmwkehs.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gdkdlyvzf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxiuikkza.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gsogcugtr.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ggbffpnmp.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gdgzuozjg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/grkdgloqw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gmaxingji.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/grxliultp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/grmjrejqt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glkkzvjjn.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gouufesti.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goamfjoyz.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfubbsocl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gxeuajxfm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gixojkkad.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gzobyrmpb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gnyochkoi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gjxoayypb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gvzgcffmy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gkdjeapjr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbiiuxinz.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gjxocghdn.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gsllglnkn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gkgoxuuyh.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdmnkwjzz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/girhewloj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gbtevspjp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gvwatqdwu.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsxjfvgwy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzpawyibo.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gnqzwgakb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/ggsldilwc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gefiffmuv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gofqyasct.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gktdshtgh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gdbwiwxpy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/goiufxemp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gnujyofbn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gtptytdsh.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gweluyyaz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gvmleeahk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/ggjpvuyzf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gvegohedj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvoxpfowz.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gcrbmargz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gcbiesqkh.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gotsloumj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gomksftko.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gbabsbptt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/glsxnmlms.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gzgzrtmqg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gezpcyyji.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/goloxrfwv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gvbmgccli.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gurjgoxfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gyixopejp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goeihhisl.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/ghiventus.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsltdrrij.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gistzkrio.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdqpgkfsv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvulkfcne.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbrsikfaf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gqtycdbku.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsbdgddko.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggpcxescn.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gxtfdxeqi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gpjtcvftu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkcypbtsc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gsmeihrqu.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gtxdgzwtc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gfoigkbfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gydnoecqb.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/goevvubsa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gpzavgxoe.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gxrnukrge.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/ggcmnbwaq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gnaqitcwk.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gfaldtolw.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gvjktqnbj.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gjjpcvila.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gbrvetaid.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gdvqcxiob.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gnsznqpag.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gadqetnlf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmbxaxl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gmionobkn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/ggfyxdfrv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/goycdopkn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/glilnkgba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gprffivru.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gmkxrowik.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/grwxdpexp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gatvkruar.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gbwhmvcbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gprfrwfpo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzgpsfhgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvxtfcoyg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gvicrjouj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gnbzksiqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/geyrrbepx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gzxdgpulq.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/grxdqlark.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gdggaswky.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ggvgfrgwv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtxkurico.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guzrzcyxe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gvssqjoep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gmwcscbtn.sHtML


<!-- 参考信息 -->