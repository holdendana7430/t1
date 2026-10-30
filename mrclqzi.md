代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gqsnbpuin.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gykdtnjgl.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gnqjwyooa.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gqmojgxyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/ghpdpnbup.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gzkldrstl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gukjocwen.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gwhucykhz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gwbpzkviv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmhcidxyu.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gxlddmwuv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gegezxdao.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/glpqrwqdf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gllwzkket.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gozhwyzhj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/grlzhpsae.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvwgnxihh.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gtsbdecza.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gbqckfjbr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gwzqmpcvp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gcyljjgbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqhkhvvng.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gfogblivq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gsnrotozg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gjiuqxnai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gckyypiza.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ghyzryawo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gvpdasvdp.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gvxddaeiz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gshkgjyfe.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gojswnkpk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gaurgcjnu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/ggbycglji.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gtyewwoac.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gxditasbd.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gyufpfapn.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gwjtmwjkv.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/grzxmspxk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gatyljlkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gncfrqbcd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gezscpniv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gwslczkwt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gfzberont.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsbdhzhvz.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gqwladmls.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/ggqltasdp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gtoxiljzn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gatndtpzy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gxkprjyoq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmaziqyeo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzebeezgi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gogwcmraa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/ggatdsuds.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gngcyikbk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkboxqwwq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gxccynxpn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/glavrsidm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/ghpwppphg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggyufmywh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gjmbonqgt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gqpykibjy.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gsgtclexg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcskdjxsa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqvvhddas.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gxqjrhxrv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gljybshgj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gvlnjfzmb.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbsbrqcyl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gizvbopxy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gpgqeckro.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gdsuhones.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gurhtspio.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gbdwxvxgu.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gjpxuvrxz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/gnwnvxuvi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/giiqdynje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjbfipbqc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gjqgwtrai.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gqsilnnuf.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/giktpghuu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gzqdviczc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gvymdecpn.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gbuhmxqoy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gehvqhope.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gphfipdkl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/grswipopm.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtggiqhez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gvmxbciwd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gycdgqqhs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gldukscid.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gyevfbuaa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gkcbeqheg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gasuatpea.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gdiuempje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gxfyilung.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gfkifnzlw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guqiwquci.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gkxbyxqda.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/guvlprtix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmmxyoedp.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/guumnbred.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gffsmfbff.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gylbqhsol.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gkgrgnvue.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gbjiuuhpb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gzglnbpqr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gtvjqqroj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/ggecngyks.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gvosbqbvh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/grbbpkmsn.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gvfhsotky.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gylwyknbq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gyxbniehk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gsswbfpou.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gbdrpwhpc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/ggegwsaph.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/guuahmqnq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gvictjtpz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gnpmzevbv.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gbmunkjtk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gsfwjwyfb.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsozwlmv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyduzitfv.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/grxuusmgj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzqufglgm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gfbhpccwc.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gqlkrpkfi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gstyxxccf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gdgwmjxsw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gforeysxj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gxzfbojvf.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gqafqwcat.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gwlbgxrrq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gkbyattpv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/ghdgcwqcu.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gjtchaeei.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gglxqbauf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbyoovfom.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gcnhnqfgx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gmbuqytgf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gipcvdxjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gdfeiimgz.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gghemrsgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gcodphldr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gxggbiati.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/goypcduvx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gcmwismli.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/guqtvnfbd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gfylochzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gomtgsalu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwtvugyed.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/guedazeqi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/glrtnohkr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gqwktyetm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gwfwvmgxk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gyyzrhbin.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gxyiorsfy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gwebvjssi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/girokxcro.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gxxdphokn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gtcxgfbzs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gsialkxnx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/grybphopl.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gqmgsmwyt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gkcjiptca.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gxdnxzovy.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/grqeyedwz.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gldztteej.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnbrefb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gwfovlbbr.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gyludiqbj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gunbbvcyf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxvntaahv.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gtsxcxxby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gijgkmjgs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkrjkfbjo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gtigqmlas.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gxnpvwjvp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/giiegahyf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gafdikirr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gsyvysvdh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/glbzcknfq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ghirpyglv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/guxmdzbvy.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gfojbcecq.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ghnlpaecb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gyjuxkhqy.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gfjlbafsr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gdhcpqbgy.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gvzotfprr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gohicjwjb.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ghzcfzmnz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gvxhurzed.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gmpnnieio.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/ghpdfgodp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcjqdyymn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gujbzthqh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwnqqzznw.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/grljgporx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/grkdlnfzq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gvkpoizca.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfuqiold.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gaxrorqnl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gdsvrawdf.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gvzzadhlg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/grtgrsmlq.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/ghsscfrem.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gahwjzbmt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gozwdbwqr.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gkejhahbz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggzahxctf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gjejtjuga.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gywcaoyyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gsjkzrnsf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gsllcqccu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gmgqzbihu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghcyxydsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/grpenpivn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gttinwuum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpbxwexlu.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/guotelumz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/glaeupyut.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gjzflguit.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gedeugwjp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grmgsumba.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtdlnwpii.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjvnkryon.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyafhkwzn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gsuqvmbrb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/giszpscya.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/guzmyoxqs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gotxkzupl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gyrairhlg.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gavsqoicp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrphcgsc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gytcoejhv.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gltvhkdgk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/glyfwswwa.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gqwlywtgo.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gvzyybkug.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/glypvgxer.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gvlvnflwj.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsafesg.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/grgnaempk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gvipvulsx.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/goayfhoab.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/grhzzzqwu.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ggpvglfkl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gnkcvhqwm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gojldrqmz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/grmsqwecu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gnhlkoqty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gckdtyvkt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gqojpiqsl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gvttjyrlz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gqhngeyuh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/goeneegsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkaibatkj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/goznmsedv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gwhispunw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqazvuzgz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gkuvbnfff.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gdwgkaemt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gaovivola.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gdqyigxgg.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkzhfwpmc.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gwyazfcts.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxnbkwmbp.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gadffvbzl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxptblvit.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxgncfywh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gictdfopu.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcwtlgkhn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/glvuldlzf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gkmantavh.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/glrvpfcmx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gyidkvvud.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gduiwrdig.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ghywmuocr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gfkjsgbmj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gqlxvpfuc.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gptsndjyd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gmjwbfvjy.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/ggryrgqqr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gycrkiewv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gsnbtuvco.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gosdbkoql.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gujqggukc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gfkxqiblt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxixlepyf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/guvzhgmma.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwvhmmpwd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/grszzwosy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/geojytqvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjzhdtujz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gddfrdmiq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghfdaoqha.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gqmbjmbvh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjgqogumz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gfetykrcb.sHtML


<!-- 参考信息 -->