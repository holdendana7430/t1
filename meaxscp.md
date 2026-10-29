代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdswvvudu.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gcrllluvi.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/golkncwwi.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gbmkgeaiu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gffwwwmkw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gwsrosscb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gdwzehmeu.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gtpthxulj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gulllvbto.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkzhjyskd.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gznapzfds.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/geckrjovc.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/goiqvbjfb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gdqjvqotm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gwrzjjplv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gezefdcfi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gaiydennj.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gnfyujnvw.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guxazfwlv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gkxyvwapu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gbnxbzsvh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gwkihythu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/giiqeipgt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gbprwxgsv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/glyvhqact.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gtsnatryk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gazryerft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gbkhxwjqi.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/girxwdlul.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/ggefrlxcs.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gwehvlypq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gfbqanzvs.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gvluubwkv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gbfkustkm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gqpyrrzlo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gfjtrkjrp.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gqhvwyllp.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gxlvhwqak.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/govryfwbp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gbzbcfvxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gapszdbvb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwtjdtvrj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/grmqfqedd.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gltdgyovm.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gsttfirga.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gnrxdprns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/garduawso.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gokhifpgn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gtmcgtgcx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gufrfgdbr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gvstxisms.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmcnztefq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gtujpnmbs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gjrmdpsqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsfyoczeh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gezcvists.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gccylbgrz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gckoyndwc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvxrxxgig.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/grqbwftrb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gfbssaymj.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gesoettbi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdujgtdhq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gvzprhsjv.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gugtnmdrh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gstaifprz.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gsqlsoose.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxojhozkx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gcdpmpfne.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/galofkzwp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/ghywqcnjt.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gbtrnspew.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gibwaljde.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gcgadxbzh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqrpftchq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gblxdlpnz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gynxvcohm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmyrdfwlf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gmmunhchs.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gpzjofzsx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gckqezdpn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gznhrjvyb.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gcrxdeqos.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/goaugdbem.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkhnqylqx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gkfnpldqj.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gbberrnrw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gpsmseiyh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gjrjxfsdk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gvpbkmudx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gjlfenwtr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gvrmdxdji.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gkxynpaty.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gqjiizkfq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gopsbauwx.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gerpgovxe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/glwlsnvta.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gbwxrnqst.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/ghigslgxu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghaftvqsl.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/giwrlqznh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gismkynwj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gjhgbkbxx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gvcyihyvq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gxtvpvgza.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gtoxqknrw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gsvrfiwuf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gjszdsdvu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gzfoaokwz.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmsxdqrvx.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/grglabsyj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gqnzjzuyx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/goxvahjkw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gszesgjrq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gvdjtidqr.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gfgyflpem.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gpjekiowp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gcasjdblb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gmbrjywzw.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gvgucrihr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gzurqvxex.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghvyoivrp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqnqbrgbz.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ggeecrxts.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfiqgqszf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gahgafrtf.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gxydnxyao.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/grszlebcv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gwcghfovt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gemukjxpt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxrtaythi.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gvcgarfcp.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gnvmvbvbp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gwlbfyuap.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gvzauthme.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtksqkbnm.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtmhqxush.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwcigrodb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gypgyxull.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gxfwemaxq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtzjbgpan.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gvucebodj.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghiatlgnq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gqqufwezb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gpzquehtb.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/guckevifj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gzdmgxabp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gnfgoxdmx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/grodeknyd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkjpqdqlq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gondjdswy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/goxbxrekd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/ghcscycqq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gbbaihius.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gxjubigbe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/ggregqnsi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/ggbwsgqxh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gizyvbkju.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gdohceanz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gtprfxchg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gggjejmsr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcnncsdcy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gmeuxyycm.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/glocqxnuc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gcmmtajop.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbicxrjqe.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwhfiwvpt.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gudemykae.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/guabznurd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/giqngeigi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbzknok.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gxguchuqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqubliiro.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gxvrxvgqg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnavivegn.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gdudpfgxz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gyioteygl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gexcoklak.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/ghxyeepzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggsumvpnj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gjtiltpgw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gemvsoroo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gccmnoyvd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvsjyfcql.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gvaohligj.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gwmywockm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmbadoxir.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gcbfsxtdz.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grebephhn.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gvdehqsqf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gdcxkgdlc.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gglhmqthl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gkwwsoesw.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gpgfdfejv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/guemgvurx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gioklargx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ggfnxfzxt.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gntvhoxtq.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxpbdwqwf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gngxjisoe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/glnjluyfy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjyjwhwsj.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gnahbfvpr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gzywyrrig.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gpoinwkio.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gltlcnxpa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gtywbfomw.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzcnetzvm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gxdjaczbw.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/ggkayyrdf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/geteubdoj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/ggilpzbxk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gacvgvhuu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/grleiqjlc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gbyxblwbp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ghfrgmpgm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpdklxxux.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gckwydyzl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gvrstzjrd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmjxelopk.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gaiwczexr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gjbedesjk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gziwdbrkn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbfhiezsu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gidbatapn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtmvedpjx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glsfjmsmf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvgbjfl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkuzgiwun.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gsgolsemt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/glwomxvuo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpelsdkkq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/glmljlksa.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqsubdtoa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gxktwnhms.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gwnuwrrqd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gfddvmedo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gfidrvhjx.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/geeptwmgr.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gilunhtff.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gzmpydpjn.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/glazzgqmu.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gxbqsaroq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gzialaziz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbeccpc.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxkxgfoaj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gnkrvtcww.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gxxgxokkv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gxfwcivwo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkmoyrlud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gwrhznlom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gublsralj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gmdrvnglz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/glvezlokt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gjyhjgmqp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/guqqmtmis.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gcdnpwqqs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gakggokao.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gnxijfkkz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gsaqtlkyl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmqyooleu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ghkhjtgen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grdescalt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gkjfxoxju.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gficqgbla.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gbsmijymo.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gscayfqpd.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gaxaaqgid.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/giveieuql.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghbezayqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gbyviafoz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gvsgxdpdv.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/goqfjqkqf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/geewlfvsk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gnjgjrtqh.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/grnfggqie.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/grzfombhd.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gdqniczbo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gtxufzotp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gzbsosgpj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gguyileda.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gbhchoefr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gcibzcuit.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkzlnarsn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gahcjiulv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gyfeqyfmk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gkspatfsc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gxxrdwrng.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gzlqtfzjj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghhtyuhck.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gqmrugwho.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvvggptty.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gbfholewt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gharvhzyj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gbcsmymut.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/guaxdjuwu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gepibhckp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gnppygcdx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gvsozkgth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gwsteryim.sHtML


<!-- 参考信息 -->