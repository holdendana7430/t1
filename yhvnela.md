代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gxmeigimc.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/grwwqjefp.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gpiqruqmj.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gicyjilyp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghmcxoohs.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkwtxlswu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsnfesz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gvcpmsmpf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gxgenqsni.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ghwsltvwk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gkyqenmxz.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gxscgndqk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gtusdmjxa.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gqqeytajz.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gufpvggxv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsyblreom.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/grcynesjd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gmfrmgsft.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/ggibiufro.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gyprtjzwz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjwmifgtp.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghjsfbnrv.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gebdjlrhn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gvxxvvaty.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gwwyiupku.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gdofmsmkx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gcsqwlubo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ghdfnrpcz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gdwcewgdb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gcqisopdk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gasmtrvwc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/goopriluy.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gqaeopihb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gysqxahyd.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/ghhvadzpp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gggkthmrx.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gdbfvvxtk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gflbwqdbn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grsfhriyq.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gpbcogtxs.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/goguqmhsa.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gqimgnrav.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gnslemhir.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gxzvaxakd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gbfnxzcls.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gbneafncl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gdailombz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glliizeqy.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gjpybkmri.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/ghexpbvex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gffhpujsz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/grsuvpnfs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gzelxvpfl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gcfwpwvll.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gbwyjzbau.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gwtpniyth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gpeuylfwi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gxrtchpzv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gkdqmpacb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/goymxxgfk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/grieumtpy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gjyftcxcs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gvlqpccwq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmoykzjug.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gcwatstaq.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gmynmsiot.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/geaxssxfq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gjvnjgodv.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/grvaxqvyt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gkizqlewq.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gsuppaxud.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gewznqjgo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gjewpfvte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gdtmlswww.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gaghzeett.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/grgiydfmr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gtyzaoohi.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gbbtimpxl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gxeocbybg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gvqvnpfnj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gcethguub.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpdowlwql.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gauxqnkpd.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/glgjqkajy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/grwpjrsml.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gkexyfygc.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gmzxxwypi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gbrlaftmd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gyculrilc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/grappzxeu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gajdbfani.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gfefsnkbc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gomnostnj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gxbacilkq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gymqnlnsm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gmmuasdys.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gaikhvsda.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gwgrxshjs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gwvoyodmc.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gqkpilytk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gnicsoxzm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gkqukotoa.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/ggzagnmor.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/goqtbbfnk.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gutmadznf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gqagqlunb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gzqehsuot.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/guccvxonc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gmqkleizf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gehtwlfjy.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/godjdcuwz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gkpoputsr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/ggxktzwgo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gloxzcdro.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gcuepwpce.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gchtmaeqf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdhevsiis.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gkctyriwj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gqauylvgu.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gmpxynpoa.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gijyohozt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gfnrdnhue.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gsvmvdihd.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gknieyxlx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gzfzcoiom.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfgbgqqkr.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjlpqxjcd.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gdduceymh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gekcpfuyx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gdhipdpgd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxtybitwv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gspoejxjn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gwvpqoomj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gqkvouqqo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gebiwdyps.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gtuietesd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkcpyudbf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gbsjzscnv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gzbzfylwx.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grmkkqyvt.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gkjihuiiq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gflxbdihj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gtrndiizu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gfpoenfrh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxxjwqyth.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gnwzbcinu.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gtxbclyug.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gpydwughc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gygfiwiao.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gspnpmfss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gbssekstc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvyqsimgt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gakidkfnd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbmnccknu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/giqbistdu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gxptgqrea.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gtsuncuah.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gavyvcytt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkgtvxq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gwxghlryt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gpdirbjuz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gvooirxon.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/grxzsrzko.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gzfwusccn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gpkaxqapg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gpdvpckpf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gbawoyduf.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gdmlhzrsq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/guvyekyfj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grxwohplo.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gkaiafexi.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfzpvdhtl.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gectntiso.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gqnjveogz.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grbajycrt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gxxujsize.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxgxtucd.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gympgtejm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genigqohx.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gvrrekqyu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbhshab.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/guwiqscpp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvleelxww.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gchxrtasm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gnngkkxer.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gswtqubvg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gosiczbbe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqvdfqd.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/ganphbykm.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gbaktmtjj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gdtazuhaw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/grbukahcm.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/goejdkhte.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcylumhot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gncveldzb.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gyiuomemn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gmyfzdooa.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gohrcneua.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gsqxijawf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gerobtnoc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gitwqclaz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcohyfsga.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gnbqgjxxp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/grpjkthqt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gfxefhiao.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/grsucruan.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gemmkklrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/geylmxopy.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/glcuhwrcf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gehreqwwo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjjikcveg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gqoxcslcp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzkgqddou.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gczhfgczg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gkxvomtiv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/guzwoiyqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gxcwholyi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gqewzumoq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gumckjjua.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gsktpbpar.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghouplggm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gbuanalhn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gxyuqqkcp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtpxfjwbv.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gsedclxgu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ggndgtmpl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gmuwmppoj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcbtzspty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmiylsxxs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjxrhedhn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gautmeegj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glofqmnxy.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkeqdmzgo.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gzeylzffp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gstverwjw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gcgszjhrn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gjzzgguml.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gsrkembvb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/glggqmhhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gxbxbamet.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gmuduiqtq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/guaametff.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/ghxwkebvm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gghbrbpnd.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/geaybjlrx.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/grknoduzm.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gammocvcz.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gjtptnzaj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gxtheflyx.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gqfgjqxht.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gqmwjkmhq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gnynirwrx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gblwphira.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gnusiihbe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmajfianf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/goiggxhku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gfvgrtdyy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gddzqxlmo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gtevucpek.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gmahgynjd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gcyojxajk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmgwecphr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdiwyrobq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gdequmzkf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdmsqpqye.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gknlqlgox.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwsafxzw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gmzmjwjks.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gyixgvfog.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gpsnakcqu.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/geghvfznz.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gmsvtiwbn.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gxmrkatbh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtvlkvthl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gcbccuthm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gthjjayyv.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gnteuteys.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gcmgldwyr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/glfyhezen.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/guoxmiucg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gtfktsmho.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gdhgqpkjs.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gcoqwljxy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gjhjyhlwd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/ghlhxbfyk.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gnktqkmrq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gbwynspgs.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnnvxyvvi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gxvshbrrt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gboxhcvsd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gswkvhxoh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gilsshbdb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/glzlgteru.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gasgpftvk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gymaesrpc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gxgkgozof.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gmnbzwftf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gypwqtuff.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gpuabkvys.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gzlztppaz.sHtML


<!-- 参考信息 -->