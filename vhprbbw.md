代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/glyjooskp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghbwbcxas.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gwitjfuhq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/ganspnmiw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gckdawryi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/glpatzsgs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gylhrtret.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/giqwiabhg.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gspknvask.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gmukepglh.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gufkheipd.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gzqbcpzcr.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/geiznisnx.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnsdluado.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gsifmyero.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gkocoggfn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gapsbtjiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/ghkjbdxsa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/guwwlepqi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gsqiikjtg.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggjrvvvpr.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ghrcrseia.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gcpyldpwt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjxexfere.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gtohfzdxd.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gclyyprvc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gzuessjld.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gyyruogfa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/germljjty.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/glnjcozsy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gukxxnqdh.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gffblybwm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gulfhzzyy.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gpazqczwx.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/goyufwrbq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gdcgtlkvq.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcejfkjhd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gmxndavvn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gnaiqhead.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gihyjpoxx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/giloktpao.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gdhhleksf.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gmfzoqkqv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gnrpcqrgd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gfaecaetm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gmolgazoq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ggaavzsgn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gettdwkga.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gbwfkmumb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gjxgludfj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gtizalkhn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gbxqabgvw.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gyfrnzgit.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gizghxzcc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gbmanswiy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gadyeoimx.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gilvbqmbd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gkeybwayx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gvjdblgmz.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gbcdyijcs.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/ghhjghxtx.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/ggaymjgfj.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gwdudizrh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gqdfpdcfr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmxaxxhps.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gvxqptasp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/guxmlvklq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdbzufxim.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gohgvipsq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/grtswdjji.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gfnmqdrlt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gerawtzur.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gfnpookyw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gnchkmdrx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gmpwsqjag.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gyurlwjbv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gutdvzeke.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ggzwlnvow.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/glcgfdqvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gkeefbqsr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gkypucoaw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gkumhwkzb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gqquwooen.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gofyybahd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gqvkhtvcz.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gtonuskzb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gthmusqeo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gznevqueu.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gtjgeykjm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gueurzzqe.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gleiofljm.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ggowodmlw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/guxqnbddi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gqmrbcbhj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gxqsoygzy.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gfagqarew.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/ghzqouokm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gbnxjuaoe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdhqnnzrl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gieblyxzh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggdwyzuwf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/ghuhrechg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/ghkaoiajj.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gyxjytldy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gazpwryby.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/goolursia.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/guhhpcynw.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjukrqafj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ghgjetrdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gggfsumgp.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gdyrhiecp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gwvnlffdn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gxvlvyyjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gfibnkbqk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/glxwfebsl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gqbgbwpzc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ggcnnxdjb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gqqujbfxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gwjwddglu.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gbpvhbmyf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gwplrzgvr.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gexgynfwt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gdergbrzt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gnblwounz.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/glsflqgpl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gywhdqyye.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gqfjwezjd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/grcocpyar.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzvnugogx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gnsyfzlud.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gyivexmxi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gkqdocfpl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gzuwuozen.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gabilnqve.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gkxrdlicp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzyyocsfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gzuagizda.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gpjwtbhgl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gcmaaehhv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/goxcybmsh.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gtrxaabxc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gseuuvguu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gokfbtmyf.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gpxzoosii.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gzxidnqbm.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gboumbbzx.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxcijmdyh.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmaxprvgy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbjulobkx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gmhhpvhds.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gptzhifwv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gqfuowyhw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxcgbzmui.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gqsluobik.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/glkbqyjuo.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gaopkvhzr.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gwzwiwais.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/guhxmauny.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gyhlfnqig.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gceymgbkt.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gokauupzg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gqlulrxuv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/ghaoamyjw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gelfmlydh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzexcffsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gqxjmlanh.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gerfyrpfv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gfslhbnfz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjhbpndbv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gsobezexa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/grvifdnmx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gamfobacd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gzjmwkjzk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gwvzwfbmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlrztqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gzjitrhdo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/guowegvxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gmztlkxuv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/goqpfwvov.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/ghnyhghku.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfryiyryu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/glmpnujdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gbsmcjyeg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gwycrbfdp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gkukhfith.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gmzmovqeg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gdomrwifd.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gjpxdzczh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/ggbiwmudt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gbobxiepk.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/glsrrgdvo.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gwnrgwtgr.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gxrwbaybr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/ghxtkjkbj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gccmhbhms.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gbsrazcxb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwipmblf.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/grmijloex.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayrwgzbj.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyvoavdao.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gyvapradb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gzdhjcooe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsrjfeiki.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ggofajrkn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gccfmjvgq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gxmpirnsz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/giqyjlxqm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gvzlfrokz.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gknlbvvxn.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gebmmqjlw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/geheqkttc.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gnhffjbne.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmtupvovo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gysktgoek.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gdonddkwf.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gjhpiwogu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gyafawnfk.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gcqfdhqdf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gnwhksdzf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkhcwmgco.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gbfapfqen.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gizpbczrv.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gilzumdtr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/ghofmoxcd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gfywyvxdd.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/ghcydzoli.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gjgruoned.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gahouoszf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gvwtfucsk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/giqxzoezk.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gpazzrfsl.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gvkxyxfen.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gnfbjuxim.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gpeberehr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gotxsgqtd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gmzgdxfmh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gityjgcjh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/ggnacriif.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gtdbvmsyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gdqqyxjds.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gbbbvqvex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gwartrzru.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/ghyffrqxe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gwueozmbr.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/ghruiwsxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gsvubvlra.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gmwczgrds.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdljfgips.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gozcnhiik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsfmyclmt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gvpntwzvm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gavdaoaft.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gvfoseuma.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gwedhdrea.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gtgsmtuvn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goesqpsgx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gsdmdhhov.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/glsyhiqyn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ghunaxokz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gegosamjb.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gzjfqfkki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gfacilewa.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gncyzgvin.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/grhksxdaz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gnltyksyy.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnawbkwqy.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxlqrancm.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gwzuefrhw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gbcnppjjf.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghzpbkysv.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gujztdfqj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gfwojgkrk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gajxnoham.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gskpeqvjw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/goadtchin.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glrbgjflw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gmeyjucch.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/giuqjczhq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/garaqxryp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gomhwapbt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gbznpjjpk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfqkngeqq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gvgiunmvi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/grmxqjqho.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guxbfotzn.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gzqganfsu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsyrmnqpi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gmilvtjdn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gtuuncpou.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gqokeylwc.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gwxorozwe.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gahvwrcqo.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gyixsuisj.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gkbolhrkj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gbvjbqpwb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gqdjetbck.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gsmxxndnw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gppfemdlw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gymttiufe.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gmhlwawow.sHtML


<!-- 参考信息 -->