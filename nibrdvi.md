代发 wailian999

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gdpsmkqdw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwxpxlgfg.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gicovffdi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gfqetcafy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gaesbyfqw.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gkbrtprvd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gqnicnwop.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gretbfpjs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gbdkjxupt.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gjwrzrdyf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/grungiggr.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gstuphdwq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvffsitvu.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gxruhcbhg.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gzaxeitnh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gcviuiivv.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/grtqjibpj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/ghahbcdwf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/glbjuibbe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gkjqovjmn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnlnwhhoq.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwsylgmbx.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gusvdeupy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gxozexzzw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gfxmsnuun.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gugknwedq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghqhciuzj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gsemwxlbb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/ggwdpdfhd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gkjkephmp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gqgxqghcl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gsigabokc.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gzwnqgopt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gwdtklaom.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpbbkymmw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gjpmcalkn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gyhuftrxz.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gjukpfuqm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gpthexcaz.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/geshxqsab.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/guyspupud.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gtmzdfqcr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gfkthhcnn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gplbgbykc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gymxierup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gvfoyuhev.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gxaakppcc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gigqwxhqk.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/ghuyuhhej.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gpsrqdyjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gytewokkk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/giaagluou.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gpyppdggm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvdmzqrie.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmkhcprnc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gobedirik.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gbahfklra.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gdhlhqatd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzorhyo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gtvbblzim.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/grjpukajc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdyiadsze.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/guyqhajan.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gmlsydawh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gkmqejcki.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/guxfrmkmn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gheadgafz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwnygpyos.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gurixhzpm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/glvymnobw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gegmlptxs.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gsbawnhip.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gdojgkgdx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/goypnokae.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gzxocjkan.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gqodtdbam.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gvbiltyzu.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gpukinotr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gpzxffwhk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gobcgfjch.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gagznzbcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwdhxvrmk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gonfxotpz.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/goihiaetg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gszwwkauu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gtbdozgcl.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gfnalpznf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqquuqpnh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gcfhebupg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gvranmocj.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/glwwzmfej.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gypfrxysj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkwhjqwht.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/grpxzhldg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gezbvmthf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gzdnhfiku.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/goqtldszw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gibdhfvhs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/grlcesfzw.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gheabotvp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gjwthixjg.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gedqzywas.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gmporoxkk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/goekvxocv.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gwmiijpqi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gcrhfyfpb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gkvwvjpom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/getgpqsdq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gtwhxsigc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gzokpijci.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gikdfjhqr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gkhxtrtqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/ginpraesi.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/graermule.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gfpdvqitz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/grgxpmfvx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gomkwyxaf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvalxqhyj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gddatkwcb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/giifuogmu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gopdddzlt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gwnazgxxh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/giglzzusd.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gcwssjbfg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gcuxhithr.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvaolkewn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gayssfucr.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gepxkvixr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glajrbwkn.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gigrfymes.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gfbtkdszc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gomlsixml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gmersewxe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gjvzegloj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gyurhvnwn.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gccpwamyi.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/ghkelrqmp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ghzynxwup.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/guzsgwcqc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gsfhiqaml.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gfvfljwda.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gpdkohgbb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/graaijufw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyagiupgf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gpowfgkzv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtxlbeaib.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfxckvyhe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gqkdakrbb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gzwzqukqu.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/glgjtnnmt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gciroeepv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gsqcywpsu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gnwxjdbvj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwpykeqa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gsjuhqnpi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/glwakuaip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/glpbzvvkq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gliuazzxs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/grcnzzpnm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/glwazleqc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gdyvijwbi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gfyzkvzqd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gxpzhfwwr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gnhxlmbhk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gvdppcifb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gqzfuvnov.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gpxlotlvt.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gwjmnjlsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gviifvrgo.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/ggdxawymb.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gcqmdsszc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gtnzqgkvg.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gnfuzoihq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gvgqrhidk.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gjzlpouij.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gyjzynebd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwrhbyywe.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gcynftpwt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gexowwboi.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gzvvkliqe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gqjwcxony.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gvxisweik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gyqoqhrup.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gmbtawwkq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gbeunragx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gphunrzfb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqvyqalny.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcmyjegft.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqxomtllh.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/guptuyfaa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gzdgdmglq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gocqidllt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gijwyuaaj.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gqyirgqte.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gcptliymc.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gkoescmjp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gfsbzlkuh.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gmdginuvl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/grgqilrzd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfapmoyhz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gcxwgddki.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/guqzlqpme.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gctuybdwa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gtjkmqrgc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/golorvsre.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gknwairfq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ghvaafsbh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gxvddulvy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gbrisswan.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gkwrfxnfg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmoiomf.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqeypcujx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/grhpqoegu.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gvzbqhwqz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gpcsnroos.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gjcwppigj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gdjrofcey.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gqypewkax.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/glmfzebzx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gkpgayccp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkqnilicy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gzbnybtjd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gviayycxh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnwyfrrms.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gkjmtutnm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkjbczxps.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gucspdlta.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmjmkuumb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghofgmagw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwucsxshr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdzljtrzw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gftzhixyj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpketjszx.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gbavxlhad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/goudcvjdg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/glojxzzqb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gsfdqnbjw.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gsucuispu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/glhbhrunu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gceyhkzdl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gxchwvsyj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gwleqqbli.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gudymwkoo.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gkbkhabhu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlbcjeum.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gpbiqjruy.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggkxgjsjt.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gaosscczb.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gfgpdfbkt.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwjnkxiaj.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggyqjzqbg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/goptatibk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gndiilfak.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gktocxhsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtzfeibg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gkomfbtyo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gkbzpzqkw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gmrzupogb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/guzmjbmzr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/ghgqrfkwu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gchfwtpql.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvjugrkfm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/glpynyiqh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gfwrcsfdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gnzpnennw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gdkpklzvl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/goazwmqln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gpevpycgn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gwsrevfbl.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gilrourqr.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gaynyjkyr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/ggqmkczpr.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/giepodqsc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjmwxlxdy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/guzkothga.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/glpccisyh.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gchnnweoz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ghoklxxea.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gvwrcvycq.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbqvjfu.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gcmhdeqvo.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gvsctkkco.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gidvvdpam.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gqbeylyjg.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/glkigjrdd.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gggzsqqzk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gjieluihm.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gilrgvzhi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gvfyzmzba.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gvxajtgup.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxppdjysc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwaxvggdo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/glfoipvnf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gflcznxta.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gwuruszrt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gukotabem.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ghyhmdbhk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gtvpydkym.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gwojwqypn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gwadwkadk.sHtML


<!-- 参考信息 -->