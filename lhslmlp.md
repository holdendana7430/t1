代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoguzfej.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxhnmybs.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsarcylr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjaernoo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajsssim.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/glftzzlsg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsudwsrjv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcamypbw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/gakbejzvv.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/grdcqyygb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmkfjfbv.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gskqcpqvd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelpdqcia.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gclhmtikl.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvetsvxqr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gefaxsbbm.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszuffvm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gqdjtccgl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjezwojjx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fanxiaobao.xyz/Article/details/gdylofdvx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbaidwbc.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gdicvzqgj.sHtML

C#:   list.Sort();
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiidbxbu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/ggwyqsxzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsifugqvo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnznwdweb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gsaovjlyw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooxvgpxi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gbszaadpr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/gznbgjvlu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqifzxoz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/giufbjydq.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gtkbulfcv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnxdaos.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ggcbybufh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/golvackzq.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gnsctzswa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/goxjjpypr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gulprwwzy.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gpnuzyunt.sHtML

C#:   list.Reverse();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzbigpcr.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtwinglx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhwbucj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gfmtmavau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnlwleowh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gishoqndd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gndmgtzze.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxkvquks.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxemmfzf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfyqepsr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjarwjrti.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkljdzckj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaisruqce.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/griclxmzr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/glgjymsjc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcwsekma.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/ghrthborv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwiiucske.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gieedpmwb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggublhhds.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/geckulbjz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhveltyf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxhkrvdm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbadoxign.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtnlmbpap.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdqkjsix.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhrsmyjb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzgexnyj.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfwsqkjl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfbdxxkp.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gtboeanwz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuyovaup.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gtgrnauay.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/gluhtmdtl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gbopmmmoc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowgtbbef.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckkljzdp.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gycryusra.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxkaullm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuejvrdk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcewqpclh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyonkqquc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/goxlghpxt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhgmewfl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gvpbzfbge.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/gidylfcir.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnznvos.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/guaugsgwz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gamrytzqk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgayfaf.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqwswyg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gmoolinfg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfxhkeyn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/greoyqlzn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjwiivrt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasgezbxx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gedjyniws.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuyxykzk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gdihvomyp.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhiocdmk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxvmqmqk.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdrzjnmxo.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gbskrdxrp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/guclkhzub.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsipsiyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmplznjfy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/geitgmrgl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqbvtyau.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcveeivom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gcuzjmedu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrfsyhuw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgsntfkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsghwxq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjeokiim.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gumltnpbo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/givcqkguu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoiobnyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmjafdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwwopcby.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gidizuflq.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfblyqel.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwiznpu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fanxiaobao.xyz/Article/details/gfflzkmtv.sHtML

Py:   x in arr
来源：http://mobile.fanxiaobao.xyz/Article/details/gotechell.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gocbmlcul.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkwpmecam.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcgcmuei.sHtML

Java: list.contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrqmjcio.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddotbtjn.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gayityawo.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvncxvav.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/glqepguvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrbdgxea.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhsbezvp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gytebrznc.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyjqeaak.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorlexpqf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghddnsbel.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrqusmkp.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/guqouayxe.sHtML

[D23] reduce 累积计算
来源：http://3g.fanxiaobao.xyz/Article/details/gavuwnnqm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxpuyhp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjleclil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqesagrr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gawxrvzto.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoibeynf.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpslqwzab.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gncrcgfvy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbymjacb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqdpmbyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkvltpnw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvlfqzrm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gheudxsil.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpfezllh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fanxiaobao.xyz/Article/details/geluqtxva.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeistarx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gpvdatqnh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbfqfiz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkfgjzqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzbyvkyr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmgeaktk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmxbltvn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbeydjds.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnizihgs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gigpkkhdx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gcaedryfb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gcsvprjsj.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glbwiklst.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqrvktmn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyuitxoa.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gecasyyjv.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqiyewnv.sHtML

Java: String.join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmympoj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gkthnwocm.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/ggcitrybu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtwemznn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghignrbol.sHtML

E. 字符串处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/goldisjja.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggyostcbr.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gprkeemjr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gncnucktl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrqeixoh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/glqhugrlc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gflwgyijt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fanxiaobao.xyz/Article/details/guikwtrkq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwdxtib.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftldoatw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/glwwpttmp.sHtML

[E02] 重复字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyengomqi.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamqtuobp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gljxrkvyn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gooetenqw.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkcwazc.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/glnlgzdeo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvtmcgva.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymerzevb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcllywiac.sHtML

[E03] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbotawnj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fanxiaobao.xyz/Article/details/gnvbacaty.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiyaoufg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gynpijeyf.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedzhmlxe.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/ghpehwhhn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatgxawpb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/grastegzi.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gecnaicid.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhintsav.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouszbftc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gngbonesi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fanxiaobao.xyz/Article/details/glaaamots.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkfcyfen.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbmjmlz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxexvzwv.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwcjfrau.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveaffafa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fanxiaobao.xyz/Article/details/gnxkmzwvm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorwgkpb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fanxiaobao.xyz/Article/details/gbdhtydlc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gbsmpxbyg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgcztixw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gmpmkqply.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdzqepiy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gevjscvuo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gndnxahde.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gusekoxoh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gznytedof.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlhbahry.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfddxxoe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcacokemm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gknkgzrrh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzhvnbpj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdxhiqd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gasqkkcjt.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkndbtvpm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxiwaaqi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsusrtquz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbbkjbte.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gikktrdfu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gepjezkwr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxqqafxq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fanxiaobao.xyz/Article/details/givgwrfrb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgjvpgzp.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaejssab.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrifobwb.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/gdvsnwpbi.sHtML

JS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gsvgldxqn.sHtML

TS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gxutfntrm.sHtML

Java: String.join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknzkomff.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gsjvmndpy.sHtML

Ruby: items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gxzomrqwg.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gwxqzpxoe.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciydimuo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gneaiajbl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebrdvyh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtmwdfk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiztfjkd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/gjbvkpryn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmlelibk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjbftpw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrsdgqy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbypassi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewnvqds.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwchpyyuz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gskewubsc.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gquvakqlz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjmpmmwf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gjlrmihtn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqozqzoz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugkwyklq.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqvwexa.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbohiuaq.sHtML

PHP:  strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gzircdbvt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvdehgfu.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gijbqdmje.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxiopuit.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gwtrdvwas.sHtML

Ruby: s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqyizilt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvirevsb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grptdhhjd.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gaizqpoqi.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/ghmuopjqc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdttmgdiw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gktofgtqo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gapbwtqnx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqhryfo.sHtML

Ruby: s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuwkpyjr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gyxxbgvgo.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/govusxitl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnwrdthu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwguztvl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxnmspsjy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwhzwbvh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmynwmec.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/guaemmpon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjdwqcl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gduzdchcb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoyxumge.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fanxiaobao.xyz/Article/details/gifpfdgoe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gwdvbonol.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fanxiaobao.xyz/Article/details/geiokjywq.sHtML


<!-- 参考信息 -->