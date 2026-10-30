代发 wailian999

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxcdwvea.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gydwobskg.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gzcdtsiuj.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/grfncoxsi.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gamvaethw.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzxhxgeqd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gjyrujgkv.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gkrwlzihx.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gjupbasco.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gvnxrbzka.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gfovyieiw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtfwduzii.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gguqzswdn.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gucgthwiy.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gchisqxxq.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/ggrmrhroo.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gamyspnty.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gtogvamgh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/giqtkggoe.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gntnjhfmr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/glkswvrmh.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gjymuhohr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsyxgbnkq.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gciuzbovs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggueuptoo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfokyokro.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gmawxfryr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gfchuqxrn.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glyauqdae.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/govimcmjl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gfrzrqvsh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gfcorfssm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gusnvzome.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gentsggqs.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gbiggjzas.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gmabidzvq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gxzezitnv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/ghktiucey.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gsztjxceo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gpnegeepi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gpyztojal.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/giloskjmm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gztxgztil.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gtgwnxeri.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gconmlzxk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gctqmhmgm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gdioxtbqv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gabaifagh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gkbnhdbmh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/goeuavwfz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/glbbmmrwk.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gjzqezykw.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gglcdohce.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gsrvthdfu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/giyqttnvd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gflhkpzlr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwluqzwel.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gijwnsbzu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gzpurlslx.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guayalwgj.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gjlcdwafr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gydwwohjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/ggqttcxck.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnobzwwmi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/grcmippai.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gqvqlkzpe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcoobipvd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gcsgoalhw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gkexnjokt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gdtahyths.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkpomrllm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gtxuyoeqq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gwuxljivc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gjbvfhlha.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gcsulaijo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gguyistwf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbqkzywpu.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gsoqqqjkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gvpasjmyk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdwdvqbnp.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/ggdqyzcwq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gtsuyhujq.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gtsytxnfu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxexxmzwm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/grnbodlro.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gvizrhuaz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gdohsgulv.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gftqfksfc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/ghdvztwbs.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gsihrnhwi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gjqdwpopb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gokberbpr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqlgrmddn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gxbbhkmoc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gzjkgjgzc.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gxnibhdee.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/geujbqkmg.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/ggrpgywwc.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gmgfzemri.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gisdqxwaq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gspchnefh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gkxcfryqh.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/ghgiyruuk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gvdxtelww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/guxacopug.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gsbrvwhgx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/giaabwiyj.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gciopycto.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gtethcvoc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gfpnuczhv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gyqldpigf.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gpevygsfu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gravpeosf.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gpglfpsec.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gpevlptxz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gloyjuzyy.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gykgsirss.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/ghcrpwtqd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/giafubzvd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gjsjslhge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gwdcebnpb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gcgpcexfb.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkndoaxby.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gbxlowmma.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gquvorlyo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gfnwtsnrp.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gtyixbonk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gkzgzzlut.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/guplzfgkz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gxqkitgog.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gogcyauwa.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/giilqnudj.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gypddxbdc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gejkryhon.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gliinlzoz.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/ghcsdflfi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gyspbsvkz.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gftpnbfyj.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpxzildna.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/golcszkpu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gygxcyzyj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gfzmlkbhy.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvlcgprkd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gurqqbiad.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdequsohi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gxsdjrlaa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gymkfbarc.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/guzzajjfa.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gsmpckhok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbhslwtmu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gpcbtvvel.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gnjselhut.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gcygqcqlp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gysthwuyi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gucoccnwz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxexhdhiu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gstdixpiv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gmttfofsd.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gjmgcdtay.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gvemdahbz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gicsnekxk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gflgjcttu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gqsusclcp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gdpmmlemx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gzuuqrxnb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gzflgjveu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gwozysyqg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gkqxfeyot.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gohlqvnee.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gjqcnmyjo.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gwbdlrdrs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/glwawyaus.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gsmylceiv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gflcvamxh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gehrfmhon.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gltvgwqgu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/grfrflzmr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gepqzyzfu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gempohhqa.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gmbfzifaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gapepdsml.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gqaqiuwke.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gucidhklb.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/geexrychj.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gwangjuxr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gncpypukb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gvpkhnkla.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gogcquswk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfpfobpxk.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gycdsrprr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmuscwtmq.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/glbtjlowb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gnibtcinn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glfmpuszy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gplnedhgs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gjltuwbuy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/galgtzwuo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gfofplhvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/guuxehiwi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnvmowrnb.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gilzbjild.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gkzhhrkva.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/ggwzaforq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gvevcocyj.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/guwypvfac.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfbujxvgi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gkvjpewdd.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gciodypyc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gjqjpkzqq.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gflkofjjw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gtazylmvs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdtixrlul.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gtrctotcq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gphezmvcc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gbohibgia.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gganqsbgu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gxcjoiwnt.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gepqzrbrj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gizdjkkgq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ggfisuuzj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gvpniephn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/guhsmofty.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gaqrkbwhb.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/girjldlvo.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gzfvokvmv.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvkeribhq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/glutjbksc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gmoqbchdp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gqbenhlly.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gsbjkzbnf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghnhtpdat.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmgrjfyb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/getoizfrz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gyunbbzuv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gvjumedsz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gauxwovhz.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/geuxlsdqe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gszmmjajo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gvuukuqqg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcyspcnai.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gscfbfkhe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxvamivxz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggjwbkuvf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtjvcypey.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpiqkfkwo.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gmgrmytjg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gukllriks.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gbtzsulos.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqfkyejha.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gsthxqflx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gttfsaaxv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gwzkwaavr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gwfqtifcy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gmaazugqn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gybjonucc.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/guwjdnjdu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gpsznlcsu.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtuqyjkcf.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/guwhinzsj.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gkdtuiikf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdystjvql.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gejkrersb.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gjtwyvppz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gvmdkdcmm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gbxeiadoe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcebccgaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gztpwatms.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/goytdxmwm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gdwoaowrj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gveqsibye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gcqwktsyv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gfswpnzmn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/giktqjvua.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmeijsnga.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gtkikhdel.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gndmuhmnw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gdeedlysv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ggliqbjxn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ggccefbde.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gngprejiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gnrijnpva.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gnwliuqbn.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gmdhfzihc.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gufhahysc.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ghbrcdzjg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gyrzqraoj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gevenirlj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gowbedtjk.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gnfnebjgk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/grnmrtwdd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gesjbwput.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gmetmdyon.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ghrngzues.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gcuegufeb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gihnrbrgg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gdyffbwoa.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/greeosald.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gktdygpsg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gtzufwfrw.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gmdpibaae.sHtML


<!-- 参考信息 -->