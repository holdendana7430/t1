代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gftdmfdyg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gqdawwmtg.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gwcdcocaq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxyyklbkd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gllzuvpys.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdlyvxgeh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gipgccnbp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gvjlnqobc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grffmunco.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gmwgailqw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/guabmzmwk.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gbfnxftnp.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwklpdmgo.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwmllcaed.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gujyqgifj.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gvweqenkm.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gcnpsqghd.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdnxsippo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gmgdgexow.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/giipjqdop.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gaxgxrvui.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/ggudragqv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gefjzckhq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzwejohlq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmmigqytt.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gqnjoibra.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gvzokoajr.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/guxnqimza.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gcpphpjrd.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gsrkwzlyv.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/ghhwqpasp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/geablzgtr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/glixlxkbl.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gmraxpwww.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwnlmbeso.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gwemstmds.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvkthewyr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gojntbokn.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gmxencnxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/grnjcxosi.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gltskopgj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gaeyjnuiy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gnaqzippl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gxhhwjzsq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gwprobybh.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gyptkzesa.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gqomkrifx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gppnhhyon.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/ghzbdwylj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gzlrfkqgg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gntwbihvx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gqgazazpc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjfwbfrec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gxdmxjbot.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gdhqrvzfe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gxvpcdjku.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnkriafzb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gvsdvzvxl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxoonverq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gvqejkcdf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gytflfivm.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gmeiqzvap.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/glydxyzmx.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gvhsbmqdp.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gxhhnjysm.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gjlsmsoyz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/glhtohltr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnzjlcknh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gutbingkh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/galgyndep.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gyhhmfigi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gshufyzdj.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gcnmanoiz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gijpzfjme.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gegsruyup.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gskehgdmc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gmrgsrjxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/goordbnbe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ggvmjerdj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtmqkzplz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gckpldihj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gkbnssqet.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghkgjxhbx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gchigihcs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gdpxdrpzg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/garnqmlmg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gragthrcg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gopumjbih.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdgkrnukp.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqxqyhlry.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gqpcyhrsb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gbqvoqvrf.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/griefmatq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/geqjnfmdy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjnmwrkzf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gxtdxwvgi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gkgqvhpqx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gpnlrmdqa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gpucoqngr.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gbcobecfe.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gmoicozkf.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gqwvzpsvk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/ggzuhpmwf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/ghtramxki.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gihezthxn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gwytbzaof.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gkjifimcm.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gsdscmzar.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gbuhnegrr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gtnwujacb.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gmlxnrjrv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtgjwgyjb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gvofobiko.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gruldknmf.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gueskojte.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gjmtaluck.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gjhkdmaxp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/grdgmvfat.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gbeacptbf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gjetqdipm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gpzgikuii.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gyykfskpp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gqlorbywx.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gsvnmgmgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxkdlqkia.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/ghbsdtnmd.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gmadmtfvg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gomobyblm.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gcaeirfqy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gbrulcxjr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/ghbubioju.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gatgaolhf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gylqhphut.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gbjyzfiri.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gogsoczqa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gsowqtlci.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/ggqscprmn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gkaszgpdh.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpkmrkddy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkkezbpuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gkaahianq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gtncgjitz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gehmdqvdt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gtxptlevp.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gcenqalqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/ghvrhogwy.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gopyzrtci.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/geskwcfst.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gybyqpgkm.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gxuvuarvc.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gbnnpbijh.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/grqvhimou.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/grqergane.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gzsynxtqh.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gezqxewvq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gtpbvuriq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gootjahkt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gtypaounu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/ghmptqrqt.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gkdcdnvnb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gahvrvkss.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gcmyjaaey.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gcompaxui.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbavbympr.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gbytrwsfi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gmiiukmel.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gduawcfuv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gqrjxchxe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gaysmcpye.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gsqfhxskw.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/glkrrdvmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gumaoebfl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gegvzkqyo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gihzvxsqu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gjgiolxdt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gbimqpjxv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gffzvtwct.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqxsycxqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gkqxjhwxw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gahjduqkm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gvcixsfak.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grhhmoxyl.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gqsovoxbl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gljerlhlz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gjtziaurj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gqaqbvijx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gmjcsnqse.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/ghjjeiyrg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gzqinxggc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaesowgg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gezclokxb.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/ghxphvpbl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdadrqesk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gsxtlefxy.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzzwbcevi.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ghdcantex.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gqvcwyect.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gknxggfpf.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gytewamti.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdzorisor.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gijigvnsh.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gsbwvzwmj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpdjfnyub.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/grcdskpkl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gjnwposjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gmtalvaes.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/golarxdoy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gusflbzal.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gopaixkgt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gcxeahugm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gvagfpzwe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzomvcuhu.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gczgfjotb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gbjlejwim.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/grzaynuqx.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gaakodjhr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gitcinnrq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gkpwyrvrm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gwmxselmq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gmglbaavf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gzzlgshkn.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxjtnztsz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gnfxdquae.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gelhwfitl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gafhmpyaz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gpnsgpnkx.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gttpzlwxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gxdnvqnkt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gajdghjkx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/ggqkjjnwv.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gxjabnvom.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/grsoidelo.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/ggsemrwsl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gzfyotabb.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggkpygrfc.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gbzaceerk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gehfwzxvg.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gtkacuvqt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ghqpgtqfs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/glzrghcqu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gpvbvhdbx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gcjhqapnx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghspacaca.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gyiwvoxnk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmdaehweu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gddldybzh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gmfgmgllo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gydgpqlpd.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gauzrxxao.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkkfoztjk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gkzebhmne.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzqvcwtfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwelghklp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gkvhkltog.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/grouqgcit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfngwphak.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtchzqmli.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gqsdejvef.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/givitmrap.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzgkhruoe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gobspylzr.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gygnsrlfv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gahtbkyut.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/ganpimvwr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gwpalfswu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gjertvspa.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ggdghgffs.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gsaqsvxhh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gtlmbgxnw.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/geiqupoiu.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glvoucjcu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbxfkfsmo.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gaasqmnwg.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gftcaeiux.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gleeqvrsn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gfemuygbn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gmwtbaahg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gwxgqyaql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gasakvkfx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gtpzbpitf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmigampts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwxnnnxuy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gkipuyokr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gczhznpdd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gyqufuvec.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gebwiijqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gilgisvhg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggtavkjwb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gepvzqzmx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfxaougpx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gzukiynbf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ginhokwmh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/glsofztat.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/glmgfnoux.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ghbljtqys.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghnkaemzz.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gexlisvkr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/goodgwoku.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gyiplusdt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gsiymuhff.sHtML


<!-- 参考信息 -->