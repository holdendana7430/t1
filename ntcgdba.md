代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gxmeulabw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmaqtsoxc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gnjeloahq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gmyiyilwj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkzhlgenz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gapuyipyp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gjlcwnrmv.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gbspmzbmh.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjrjtiumc.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwghkximj.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gnzimvqoy.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gbyipcaqt.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/ggegtfimn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gnqkgyhcn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gixvalmdu.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gzlsvtcfi.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gasdwoyri.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/ghzfrlbht.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/guhljzbyk.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gghpmbkxs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gkqvjfaiu.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnvmcwaee.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gqhjcycok.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gkgqkgzla.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gamxqdger.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gpqjbjfis.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gylmonuyc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gjzshodfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gmvzadice.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gzduiggct.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gscyiomkp.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gyxzgkmqu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpzivlxep.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghxszhbtb.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/galoknocv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gdwxzaxyq.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gimdffuvm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gidkzafcp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/grvvyduaq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gedyookob.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ghpbcdogo.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbcfcsftz.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gysfsusnp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gqrfnxqrn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gqishfehh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gtbfvylfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gdcbnwiww.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gostspbvn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gwptlacwf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjfvuum.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gwibzychp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gqzopmivd.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/ghmvxnaxc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/glsxypjax.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gvvfgmqwm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpnzshpr.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gtipaefwm.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gpjlqmdcf.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gjwqbucaa.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gqmmtgxgw.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/grzvdjath.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqjrxsriz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gaahiqvft.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghaoggfxc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gmkpxyqai.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/glzaseurf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gcyeoardh.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvvdyajpz.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gspioxvac.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gbjvgctak.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gnsijsbgp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gyllenuch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/grynureai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzdzgxyd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gohgwotml.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfgxmgxni.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gflymyyhn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwphvhzfe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gfjfncsrb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gppaowllo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/glasawurd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gwcqwworn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gjooewifm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/glglmnauj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gjsjfhlqp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gqmtejnjg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/giuynyyyw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gudipgmve.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqpnfbppm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gruqdiorf.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gcbzonjrj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkxkyblnj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gplatwbkm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/glzqsxhyb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gqvsrqnrt.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gynbwvawz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/geothpncp.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gkdczchur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gqzeuxulh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gdsghabfw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/godavvhpf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ggakadqxx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/geissdkuz.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gxuxdlvlb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gkelbfvhc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/glqkapzcq.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/giduonwla.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gojjmbbsi.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/glezsogrz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/ghycxrbkx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gkoyrcwhe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gaxflgcif.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gonyxfunw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gfllycxbs.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gkpkbpgjh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gzcbbufgn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwzwqggtg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gjegvxema.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gddfitcan.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gixiaulkd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gvdwruojf.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gwapwxxxh.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gnqgziuyv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghacibpfl.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/ggrvdkuzb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gqjbovrju.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gcwatvtnz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gqewbscio.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gkweelbxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/grlcwkazo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gicotdllb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/ghhvnumpp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/grvixaokn.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/ggigstlex.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gkvreixgh.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmkbppaiq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gclrrksfk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/grcoqscdu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gnmmbqinr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gageodnvo.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gkkvosafr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gniuipzxq.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gehjqntfz.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gzgrvjbff.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gatpibfpr.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/goafecnmz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqdjpowsd.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/govthrzvp.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfddhwpag.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gblaumlmo.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gahvypsvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gsfclwxac.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxmmtfmaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gwjseifew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gsqfmtyqh.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gfkjpkeps.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gpcnvaszf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gsuvmpswo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gvnqaqtox.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gffkrapow.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gaxegmznm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gttamfvpu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gdijtxhyf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/geyhfcfdo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gziovgkrf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gizplgnif.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gjkxyovxc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gjaawrhwe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/ghmhdvbzr.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gtqapeyoa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gvwflfols.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/ghasvmjle.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gioyculum.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnqxklqva.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gctbatwvz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gdnuhtltp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gjhduzqwl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gnnyucxrx.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/ggsnsbdnb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gdwojhmwo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gsvbwznpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gapjtalus.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gveqkxnta.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gejlhahch.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gqnokeiya.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gashggwzb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gmrnkfuki.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gjmbbzdgu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/garcerooj.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gclclldyp.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gezdpbjgz.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghyncwgdt.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gokbodfwe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gkxclapzx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/guecytubd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gwxpabpmf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtqbhfyaw.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gejaxqhrd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbjetiviz.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/givtsuczp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gcmuhkbmd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gnkviopub.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/ghsawpohp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gjiouoycg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/glqikmhxi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gvipmqikm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gmlnquzln.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gycmhpois.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gonkumukx.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gqlokhhcw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gadpdzlvy.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gvojaqtht.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gmgirapko.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gpqoqeqtb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggejbglpc.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gryqdcyls.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gfuztzauv.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ghaxwijzo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gotwmiimg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/guuijdbbd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmhapdeou.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gyhouzchw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghnidqzpn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gsxoxzoya.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gzgrjmscq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gwejsuefq.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gmmqfymvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gihoghlng.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gwjhxyxek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gmotrixue.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjwuxmxvi.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/glmfssfde.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gzaeludjy.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gndtibvww.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gbivmnnxg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmrpsnp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmbabjamu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gvvypocve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gvfmiogzs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjaxnvqgp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gsbyzmcrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gxaumlpfh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gbnsjbfis.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/guyeruvft.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gwairmlrt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcbthkalz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gavpvaoaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgyywobb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdqxmmnil.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/glerkgeci.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gqxaquhsv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gemlqzqzs.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpjzpehyt.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gjdjstjbz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gfqjvtyql.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/goalefssh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gumgiausw.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/giaanierp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gspghmaei.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gydliemus.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gpbbovwgt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/glokcgtbf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/glbadohra.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gtudgibja.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gnqpwlrpm.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxaoyizws.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grvrxrnvf.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gbxbfyrsg.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gkvfkkmby.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gdkntjcli.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ggmdvgnug.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gpvgqftdg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ghrcmnwxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gtoohiwzh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gratyfbco.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/guijcypmu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/guudlxvtu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/ghncizrjr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gnmemvsan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/ghrpqjvjg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gldxtzptn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gcexgpffe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gmumufhgd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/garkhxfjr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwzlarpry.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gpexfzkqi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gvperrwhk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gczsetfxm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/ggdnewkip.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzxvywhoc.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gxwjjtpsr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gmucnvdht.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwvzwbdmr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqnnubtwt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gjwwmcxjw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/goaxwevbe.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gminpokrs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gdqnahxsq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gugaczogx.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gfvioynan.sHtML


<!-- 参考信息 -->