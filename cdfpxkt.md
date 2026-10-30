代发 wailian999

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gsbgqtwlx.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gupmswrnl.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqdkuscds.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gqjzrlody.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gbmvedxcv.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gumgapuus.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gawuvbnjy.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gshuhflmq.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gclmarjir.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gidmcwkdq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/glkngaxsj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ggyobelat.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbbzyifse.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gfwwptqgm.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gaofkridk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gyxxlpwrc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gufbymfsd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gjbxjuxmh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gkywlwslt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gyjakolfn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gcwaizbrd.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gdkszuclu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gczgxbarr.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gyrwnbfge.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gsuxvfrps.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gtzrsaest.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/glyahpmql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqynnrxed.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/ghapmoqmu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gmbvudywq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gltettcyt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gxzavfmju.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gyokxaoud.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gnfisctiu.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gtmjjpnlo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gnkbzkzjk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gmoedyjst.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmmhvqtbq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gwjxlpnyc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gocpepdom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gbyxgdtfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gbqbgqyvw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/glojecgdd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gkwrvgtum.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gsaqyxolb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gvigfeeto.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gtrrczqyv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/glmavaxfc.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/ghdfqkdos.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gcazjuyhv.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gneajxsoc.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gywwpegez.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gvzwenxaw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gajfgesty.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gejvbhzjr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyicsnhci.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gxnvcoevm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsqgcjlpm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gjsnsasfp.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpdpcqulf.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqhigzpxt.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gzlihqttd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gbijyiisy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gffdqdbti.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gojsbivnb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gazdmiljq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gpkgoyoae.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gmkvyrslt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/ganavedrn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqctytil.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gblgrvypr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gcqhqhobt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfcnylbcl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmrgbomvr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gasiuirrt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gipongtwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gawyjxhsd.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbvgcgoyq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gfqkldlxr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gltwvzjen.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ggpdrxgiv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gyayihmle.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gsogaqrks.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/geasapptz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/guaxbdjwv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/geckeggun.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gzlordsgk.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gcuqqtzvo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gbonjtwpe.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gusajvwly.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/ghbdkblyh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gewujlkzf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gxwlguoum.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gokmiygfk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gpioyvkyc.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gykgqplbm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gusbjwzjr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gffaovfad.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gwytrhvvn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpqiksszw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gtvfuunwf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gfenjgsdy.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/ggrqujmva.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gvjyoocby.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gqfngprcc.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gpfsmrvnx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gqykrxipa.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gvrmrgzcm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gfnorajuv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gvhzlsqcj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gketxzhrj.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gdhzqlktr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggdcdglpr.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gaozzuler.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gxrhrtwej.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gutmbevci.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmmevyzoi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gpznydjcx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gksomilnk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gbhttdqub.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gqffeaclk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gsblctybd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gozeekytk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/grnequwkr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/giouwulcq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gljtrzuds.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbwqoupau.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxoqvkyur.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gqytttuiy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gjoeqvgdl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ghjcnukdc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gganehnfo.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gnaluzjhw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/goqltdydk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gjyeugxyg.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gkycunvfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gutiaxntm.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gftfizpur.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gththdmbw.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gjoqdstso.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gltwsumat.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gcxllmkgr.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gqpjlbdtt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gcbufexjp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/guqwvkadd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/goirfbpwx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjoghdkrp.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gytrlvyik.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/guxjinvud.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gobafjrlv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gbbcwlvqk.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/grzvxkwgj.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gessavnsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxpkcjvpl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gysflecyc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghskefwcz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gdhftzexj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gwwlcsotx.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gwshszynl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gkhaolube.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gjokvfrty.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/guyvrgrbr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/godznciek.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gkimicnzi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gfgsrzeap.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmximjfxk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/ggfnvnqig.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gbqesrust.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gycsfcwij.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gxluiuavl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gmicbugdx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/giamkpbvd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/glyglvlrf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glokwvqtt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/ghqnfezxl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gvimogorc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gbxwruhgf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gdrivyguo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/ghuoovrjr.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gknjhbwim.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gioujvgqd.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gaxzblcdt.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grvylzkww.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gdpdbbzvp.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gishayltd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/grfnwsyaw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gwfbxvunb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gfgwvxwzs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxorifsdw.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/ghugzpcim.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwzjkroi.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gkitipfhj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gsiutpwrv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gdmvytpeb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gpsnjmerp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghajezvls.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/guiovjwwj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gctuynwmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/giwbqcikp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbpjzrouy.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gntqegosf.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/giwbzuygx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gsatghjom.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gnuwotnbg.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gnnqcjwoe.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/geoovfsda.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gippmrdea.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gvzpskslw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gcuowwzwx.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmihmzn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gzbltzdsi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/guiyihfor.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqlmsubew.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gimbbbigi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxvxhvumd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gnridfvvh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/glfxtmnqu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gnbhdvfyq.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gxisynfai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/glzdcbowe.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/ggldwxqni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gmhbtebfa.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ghvhbygkv.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gjlcqxhfn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gaazlvljz.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/grsfzevzm.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzwytiuuo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/ghgpjdfcz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gwrnqgxpo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gvsrgluyq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gglkywpcf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcscbiagj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxtvuxzcv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gkvxcchjg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gylqktzwf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gecivheni.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gwvgyonxq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/ghwvydqnk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gfnyoyzmw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggobrsrfv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/godlebhox.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfiubpqyr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqcylumos.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkedxhrtf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjavdpzkr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gmzdpkupx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/grtqvkczk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gvdyvvxsd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gehhgigdq.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gxgdebpzr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gxebfferw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gsfaofajj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gkuefhcwt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gnxplumgw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gookavyrw.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gnpsqhrji.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gfmliouge.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gykggubei.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxapbempz.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/goycnetlq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gfzuzpxjx.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/grausegjr.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gtvtxfdfv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/grpmixsrg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gdkmsmvle.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfodznfdv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gcqlldxky.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gksvbiojt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gfefaayoi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gabfutttl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grdrcriat.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gqqtkndfd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gttvfuqnl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gidmglkkv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gcmooopmp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gmtamvswe.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/girjbawji.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggldyykji.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gtbkhumpb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gdzvytotn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gyigiexda.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gibtsdvyh.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gsedlmosb.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gljvtualw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gssoqqohl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gxpueobhm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/grkefieji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gxpetjcwj.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gnxgqhwdt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gkozdylec.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/ggdrauvif.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gyowmgfzi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gypljpcre.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gxrxmujxh.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gnsuksexo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gstblmbgo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gefuakcoz.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gngqqvvcn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gfrcaydye.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/ggbvkzfmq.sHtML


<!-- 参考信息 -->