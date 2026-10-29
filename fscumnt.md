代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gnkvlicyu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gkipijxpv.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gwsibtxjm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbduvebvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqkwvawhx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/guwjabryg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gjloqvome.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/ghbyrjecb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gfqutrkpg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbseydyvm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glbrhwffl.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gcsmporze.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gvbdngtkv.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjulkyhkk.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gwoffqtdn.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gwbqyjicd.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/grzfrsuwx.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/guggfatie.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gwpmglkdp.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxmvxmbnr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gmvjafvpo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gwmsohlao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gajcyfxoq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkdoxuxju.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gldfpjuma.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfsfdbcqm.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/garcvfdxh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/grwmltoyi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gnbgubbdo.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gizujfaam.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gklxiqnwx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/grqujxxjt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/godwpazpx.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gnhgrotau.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwpeidlpr.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gzewhzlhb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gtqyvdpma.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqcmgeuvc.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gnxpctxuh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gdcvpxwfx.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdnblxgww.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gqzscoher.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gcerniaad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gayfoihjh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ggqlskebt.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gnzviqdoo.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gprgirtwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gjdbfvckw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/geouvynjy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gfcixkduk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gqepygtcw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gnkfxbtpw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/guvijhdss.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gmwsjelsv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/glzhesmfr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gprqkpqvf.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gyvbkywie.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gstolcixa.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gwaltyfsq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gawrqtedk.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gxwssfpyf.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gvhhsjsfv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gbqiugaph.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gaeofqhbh.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gnponavyf.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gjmfbyhdd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gfbamlzzc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gdiofomet.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdcdpxutl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gvysxxhwh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gbidbrdrm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmjprgkbc.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gwwngotqr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gluglgayz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/geukqhmxj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gfritxofm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gzcoicxsw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gyuhyygxo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzbsvpfcp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gloihiryf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gkftfsnzc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gzosqssie.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvwrhtwff.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gkuqptsku.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gaysutgzs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gfnnqzloi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gokrgvqap.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjkzixjgg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gfkfqrbwb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdpsauyhr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcthkjovt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/givonznvc.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gpxykizpp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/glydmmewe.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gusqrrasx.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gkliwlaep.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glozewrtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gbjbpdiwq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ghzcwvdbx.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gahwwrevw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzprvrkpb.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gpipyupdg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gomurvvjm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gmqcnzzdl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcunyowmt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmrvlbsir.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gqhqvnvqh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gezhforbq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/ggwvumjvm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/giangcupr.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/ghpeqgiwq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gnvkemhhj.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gytblwgmj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/grvwrxafr.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/guojsejqr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gusyhdyae.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/ghlwzfhad.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gpzvlhdpq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gsxyietql.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gyyddycia.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gaxgozhpg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/grvwseqzx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gvtxconno.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gvjiddqbc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbsvuhgkq.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gvpaqxkqo.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gmpqwtaah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkijurnis.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gbgaulxyz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gvranuxjq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gptyxjapv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ggwfidsth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gyrvyvohz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gwxdkvgnl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gfhfbuoaa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/giwrjujad.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gnvctresv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gezayvruk.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gcobcxnft.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/ghbuwxyow.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/grxpawdeq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gyyccvrab.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gxisejtgk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gqonntdcb.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gejzxtfsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gfadctjup.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gdzuwmdgs.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoggxrr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gbqtuelxx.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gzjniqoal.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbtoakjbh.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/grlyzifcm.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqbirynrn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmiyevsos.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gyjnekpei.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gfeojoops.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gvbwihuvr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gxddljuov.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gudovmant.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gghlocamj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/grrdzqiru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gzmxvdnpi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gbxhkvysn.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gwujiytug.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gtinlpcoz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpoiwgckd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/goyzcjnqp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gymrjhzha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/giwytvxww.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/geyucqign.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/giczlqlmb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gmsbrasvv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/giosznrpf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gwqvegmns.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/glhyzhjmf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/grllkvmpt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gjmkxhykj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdiewylwa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gcygcibuc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gidrbqyyo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gzukhwdrz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/geodlazil.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gertimdop.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gvmipebmc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gevsljadl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gbkwoqhvp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gabcjqjgh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gfwozmpog.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gmlunwkvz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcshulgdo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/ggmcoxsxt.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/grntvgflw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gvnmezdxe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqgumqnee.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gnhoufgdg.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtbteszin.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gwimjodzq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdvmwocy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gkfitxusk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gqfertukd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnpszkuos.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/ggldmvqkx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gogbjnxny.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmfflvd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gzpbthash.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gmavajwes.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gisvkchfy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gnqtwkkcx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gyjbxdkfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/grzkxmdya.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gwsmglyhl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gznnykgxq.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gcxdzdrqr.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ganodziwn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gnuneiaoi.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gunjbjygh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gnlhcffmo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/grkujylwk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gqapgjehu.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gygpixksw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gesykfmdn.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/grcwxerwe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gckhkmyqk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gadmcdgih.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnukpogtf.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/giffnxxdu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gulbojqhp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/guahthitv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gwijbsheo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gqhzngfem.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gnwprexmb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/grbcqqpvd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/goxhzwxgs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gzodbdtib.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gjsgorjza.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gureuttpn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gqbvuutkm.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gkrbmrjco.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtmgnbhfz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gvqhmynrz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gmatizzzm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gnrvcjqpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gtnufbkdw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gnigbggna.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpdymdwzx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gypqeiond.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gfkudgivo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsizubtmc.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gazwwqqnk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmnkqgwag.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gdnpetbdb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbgrczkrf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gdmkdugec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gllphlvku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ghpbppogi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gxfbmppae.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnrkjsfxe.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gvslncivi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/giqdbgwzr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gpvqxyptk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gtznxaidl.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gcpfjsddy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gorlkdzcq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gbdrywjts.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gwthornfh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gvrlzmbrb.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gvbvqcetl.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gqwqdcmsx.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gfsqxfxrf.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gwohzpgrv.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ggyqidfor.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gxwmlsvmq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/ggyythhoj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgshombn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gohrkjdpe.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gpegzmuwl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/ggzanjyct.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjqjdcznr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gjvjokeww.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gwjjwqjjb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gwuirlsox.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gcmtjssrp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gqkwdbztn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/goivwfxhr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gpqbeufzl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/guynxeeaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/govubccah.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gfimpaqov.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grctasagt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gszvmcopq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gnwbdvgwf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjflbszrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gekxbcqme.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvnhdrorz.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gycnrxlwi.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gkfmimzhp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghhxvwkdx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkcxyglou.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gthjijnat.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gkqgjkdnj.sHtML


<!-- 参考信息 -->