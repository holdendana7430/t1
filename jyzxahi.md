代发 wailian999

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/guiwxwhsv.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gdnoyohwf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gwfxxwtqv.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gcpxsalqo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gvavidyga.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gujuihqae.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gehqwqksu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbzrxigez.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/ggwcloldy.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gcmmuhlag.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gxuhgnemi.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gsvmkquqq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gbrudkxdu.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gazmnyqlg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gbyuzcpfk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxiqbdsog.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gylihnbim.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gayxrosgw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gjtcgqflp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gnmsugrpw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gyaazjsqw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxxhuqtlx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvbrwye.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glvtwptol.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkiheyoyx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gthugbgka.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gqeiyjviu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gqjihdvlq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsvunpacm.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ggnrwvjim.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gpvetwqrp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gwvovtayv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gatzmvpht.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gwezqtuzx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gtntkmhky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gfhsfvfap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gvxrmoqmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gcajnybzp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/giolzrwim.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gqkvedpdb.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gynxnrzlf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/grdwnxusw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gafhqdpxo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gljimzolq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gmdseycmw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/grwomeuug.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gairbsxku.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gtsbdfgya.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gfhsvebng.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/ghybwestl.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gmbtfmtof.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gresgxudc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gkbdahkuu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjqjjizng.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/grrrhgbhm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gublwalrr.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gklmlsyho.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gkwnenuyk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gcdwsdmtv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmrciihch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gonkgikxw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gokjbglnr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/glmomcsfg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guqljeykh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/ghyfskwdh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gxzjylkfg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gwwjrweji.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/grpnwkteo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gsllaxhhe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gkgiooeyc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ghhacygkm.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gyqvfqkoi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gmrhkhrfc.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gbpynsxpw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gqcanveot.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gyeozhcwj.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gaqbdfqxb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvbmtvo.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/guhrgpvkr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gciwofmul.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjkwpxelj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gyydwwhmv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gniehdddf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/ggksjlevg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmyspbspr.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gjsjkdrkl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/geljbdbix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gwsjdyeec.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmbhsjufb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyqljpids.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gyrtwwpcg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gqwlblddu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gkzhgwwix.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/glzevqauo.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gfrmllnvz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gumfbhlpy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxozbcmal.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ggclmfuhx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/giumookyq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gysmwbdzh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gcrtcuhsv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gclghkcip.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gassativj.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gqfzywgkm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gvgaqynid.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gyvgoxkxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gmayueqqh.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/glctlhdzl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gweitmndp.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gegjwoqfc.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gokxdpatm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmqwgcmdj.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gpvrqymod.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/ghdkaeuoh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gcmmxqohp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/guvhmjihk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gtmdfpmup.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnwvgsmon.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gkcnznenm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gkgclhvxk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gzwvxuhbu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gezrukmtz.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gjyzhjvgs.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gvowhehll.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/ggpmiipor.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gjewewvdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gonkpplsr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gfpbycmbe.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gbkxzbdeb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gykqsovrj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gpazisavw.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gimsohanl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gbgoclvxl.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gqxifwxpn.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gsrbraoja.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjfmwgybu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/guqmcvwed.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/grwqnnmkw.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/glimuquxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/ghyczkidf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gkodfstdk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gdnwgsrio.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gzqhcrhlr.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/giisgxakd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/ghcgxvyix.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gzhireodl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gsmjhhpmv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ggrepanit.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gzxjihcpm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/ggioulabz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gpvvrirfc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ghvljfdzv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvitmewka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gpxgfdihh.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gnhhyydfi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gudkeolkg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gwesbycgz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gyskkztto.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gfnxttpij.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gygherhoe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnnolgdq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdzfkgocs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gxildtzhd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gmyuqzfkg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gdytjozsj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gaqyoynuu.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gtednbeyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gyteazzso.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gjxjbtjrr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/grtfpcvgk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gctecsmec.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqdgxjwih.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gbxvwarls.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gpoueqdnr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/goamquhlw.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gcrxwhtia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gckvbymjo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ghekgizbs.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtfgkwvih.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gnzrxtbii.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gzqkvrpxq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gernmgkkh.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/givomvrrf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghnodhczs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcmqnypsw.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gpgobyhha.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gafpccawg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grxjjvnvs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gfzrtnasz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gfatsiwox.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gvsdwrqvc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gebdwglpr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/globnlhzd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/givovlgbc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/grhohinsj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsdaoihof.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gjhfkotze.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/ghldtopce.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gxqljyifj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbztufdww.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gadezsmnx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gllbxahyb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/grhzwznln.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gudwvhetw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gsomvpkjg.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gnbjosffd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gpypbgwkn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/goxkrrejx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyrjroflj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjrmpudtf.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggyveryey.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gouggmemu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gvxgdsdbs.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gmcptdebf.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gqrcivude.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gzxurjnzc.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gsnqdnluf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/goqrsxvza.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/goqqlgtmf.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gqyyeytmv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gxigzqhbh.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gsdpzidqc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdhddrrxm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gvpuuihfi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvfkpqngx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gtrrxamvp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdgzvvmhz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gqetqwjxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gojvngwdd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gsnpggeas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gjanrmany.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcyipccoe.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gplhcnwvm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggbexrltn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gbercbqfp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gpxbsdcht.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnivnwria.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/grkwhcfco.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzxayfh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/guynantla.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfzkbczke.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gdlavnhog.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gztbjvtac.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqiwxlqbx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gpdydweeh.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/goliafule.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ggxxhctno.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gaxanitfh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gieftzamc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/grsogbroz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gcadlbfut.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gsnrglnjz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gohizuvyw.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gtedhmlum.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gxbowxwgw.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gkqmkebcd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gmcudufhd.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gpuffftru.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gkaovbprf.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gzcwcqqfd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/galouyelp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gesbwsuik.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfwgpvxtg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gzwdggwxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzzvjsgxi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gxrrknujm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gcdcqktna.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gwzmvgeov.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gdgyksols.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggnszfwua.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gojdclpfi.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwkoifwap.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gbqystixv.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwzwrhajv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvceiayie.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghkylhjjy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gprolttiz.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gxxpigeyy.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkiypsfoy.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ghtkiidlv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpvpqlptq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvekgxk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gcubkfmoi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/ggalkfodr.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzhskwnju.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/giisqnmfj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gygnosxiq.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwtwhlwvv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gfhhgqcgf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsedmfgdj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gkpnsrkel.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gqrhdxegr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvlurel.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ghdoiwfjr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gswqskpoe.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gllrimueo.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gbeqmgzgn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gyovqdsew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gfklyxbvl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gwwpipqjd.sHtML


<!-- 参考信息 -->