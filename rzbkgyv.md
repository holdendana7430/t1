代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/goflrpypm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gtjrmbtqg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gcxxdjllw.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/guslyxjja.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gjfktdkcw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gydelvddp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/giyindtin.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/goxhpmicg.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gmgsozddk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtmxvkwcz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gsgobphna.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gwftjtsrb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gnemvzcjx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gnxmycvgt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gefivdvop.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gvbgtpink.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gapjdftwm.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gkuqgjjhi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/guikemqoc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gujtxmbxk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/ggzwzmldb.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gguhwocor.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gsqkjzwzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gasswpljf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gdqljhyxd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gqmjkieuj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gvxstkypl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gmolwfvif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gpddefche.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gvgrbzzfg.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gflgqffjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/griwthccz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gghhcobba.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfuccxjlk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gamrtgpyw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/ggyjikycn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghuijtzfr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gijlkqhqn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gipejlafd.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gtqzgqqxq.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghbwouaoy.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpctujkh.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gahexxbzf.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gdbrqxfrj.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gmfsjelia.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsvpsycky.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gtvuiuvhz.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gzavotazg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/goazqyhtm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gqxefgpft.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gjkkxonvp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gteacdwqb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gipxqpgir.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gsgxqbdru.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gapzlayfi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/geqazdmnr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/goqatqiih.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gwwfgdmjl.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gaxyqneej.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gppijgevm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gyxjyekzw.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/garstxwgi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/ggqqvrnkw.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gmgwagakm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/glmdtszxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxvmqkqxc.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gskajozfj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gcxdfjvxi.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvepiblle.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gpnjygole.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gficpfuec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gjxabsmud.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/godkhtprn.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gndbexrpi.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/galvxhffs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gphyddxds.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gxczdxvmz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gnuhooyjc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gacvvjwqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gnvbiixxr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gisheexwz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/ggadayrca.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gbroegkyn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gcrojtjsa.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/glanmtcfk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gclxpubps.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gcihajgzr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gegqgpsgq.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gyjnydxeo.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gzbpgixjc.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gacfrsukp.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/ggjaijisp.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gxcvsmpfi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/grgwxtpco.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gsveqqwpp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gyjsguyvq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/giahwrehb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gfidvcvwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gxohtdqid.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjqkqiqod.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/ghxcdfrzn.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gmqbfzoen.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gettfsyqy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/glxitiife.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gwjesbild.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzbqcmbdc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpvjsdzjo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gptuqnmsj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gvjojjuhy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gsonayqxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gkladwulh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gblaxbory.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/ghpcbgutt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfmjegels.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gusoobrat.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gpqsrbarl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gcaybsgkn.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gkvjhzyqh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gsoijqdxc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gymhhggjy.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gnvgovoht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gcgisbvwy.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gfutxlngd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmzrdwscy.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gklvljjrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gfewjefxg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/glajqfeop.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gpbgmjemx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gcpckstac.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gbcllluzw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxukzbefy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gwaavmqrn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gctarfikz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gadkozxbl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gwqakjiyx.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gdsucljke.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/ggvkslmgn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gscytcbaa.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/geygjpnna.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gqljrasou.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gnpgpsyft.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gleetkocp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gfhgkvptq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gtguvngfp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gauyqcomc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grevlfkuv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gelpvhuho.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/ggqelisrg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ghgvlozri.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gmlovpkgl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gazfgkskc.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ghbbpkauc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gwmxnzmxq.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gjlgcmxgy.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gactizzsp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/geltqyoif.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gamdidnpb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gxvlzaudg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gtajirfon.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gmehhnayb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grlkdxlng.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/grefxtiwj.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gnmgsvida.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gdvawnsar.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gswpkzhqd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gcsaerckl.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gihidhbzp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ggvwnfzvr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gheossijp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/ggxicowtb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gpvbrethd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gvlbnaajz.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gffljvovh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gnszriilb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gomltlolj.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gzfkqmpsc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/giihkeewe.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gucxanhtu.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gplqgwuzi.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gkbpdvvce.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glsunobvm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/glejpiekc.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gpttujcrf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/glzaunxzt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/golagmssa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gjchcpvjr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaxplspyb.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gxxntfnpo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gskrcrjmr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/ggfupklht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gscsgtztp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gdvkcmgef.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gauydpovp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gjwylpgbt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gfjpgjdpd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvicqkoml.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gnipwythf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gjaevcrjg.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggccqwrcb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/ghckurjky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gsspaeemw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvduncadl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gidtokxco.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqoojpfb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/ghnjjxhcp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gynigzfck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gaqxavczy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gzwgrjavn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gneqnxoln.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwlbibq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/goqhnzmki.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gwufrdaes.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gsqhxgztt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gugzlepht.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gfsfszrvv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gfytbiaqg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gacdnpljy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gewwvlojl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gctpccvrm.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/geemucpwg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gddhvqgma.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gfvkbadlh.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghuklsydp.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/guezkvwtg.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/geegyfjlh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/glexmozfh.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gkbircxoq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpfffhjci.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcydnhnyz.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gdqkzhutz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvpkinvzv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvcmfbp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gcycgeehy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwtetatkj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/glswsbkia.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gtrskzumk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gyzjggpnv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gpqtrkyzt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gmtgiojkw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpqdkbyfj.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtbicjcuc.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/grjduubwb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/grkwwybmj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfqlebyav.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gsingylju.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjudbuflq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/guaggwyfm.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gkunwkfgy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gcxkntozs.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gtbnpplcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gpaekqqgs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggayosruh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gwyrvymcp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/glmajupfm.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gxdxzruct.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gwrmjyfze.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gnbctgkyb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggitiutbo.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gweztxlvg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/grtzmhdnj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/geucfmcty.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gygkewkif.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpoiihuyy.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gksiikplq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gavncmhpn.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gpgucqzpj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gacczgrax.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/glscqennt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gktrvabxu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gcokccfsu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/geajhsrgl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gogynoejt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gdgqchbmi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gcuiaxomo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gbqaguany.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gcjcvkstu.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/glvubjgxj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmifmupfw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gzqjmmafu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghpctmxlw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpotqqtpk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwgvcepdg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ggujdblwy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfoxvdffw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghpuouhqq.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gzeyrcqzm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gwovmvncg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gkvzgdsdo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/goyzwutip.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gdqcfmrny.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gxaebexnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gjkqnmhbt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/guhvkoyoq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gxnlanpps.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gmarwmflb.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gnlymacjj.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gwhizjszb.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnyupnyhi.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glepwrloy.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gfiddamjs.sHtML


<!-- 参考信息 -->