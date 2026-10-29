代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gupecbhyk.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gtjvhjfuz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gysxgjulc.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gooyudmwc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gcwjzaffh.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcvrcytge.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gsmocjuhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gpcpqfzmx.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gipmqjnrj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gqhuuxkdc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gysomhurx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gjsbevupn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/guvtokqhk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsrnrkzfc.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gagbvadxo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gquuecnen.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gbgisunvq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/glhbfbgsj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gateztacy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gujfkiyhs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gwqcmrxje.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/grkeuqvlk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gelfcditw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gmzcadoap.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gixngghvy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gspskwxvr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyrekpyya.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gsxblkfeb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/glvahgber.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gxpmfufyf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gtwsiyazh.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/ggnfljtkw.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/glfbpmmpy.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gipijgncc.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gzexbthuc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gbatwsape.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/glllcranq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdejptezs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/grqjsojje.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gefdztvad.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/ggjxibwck.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gkmfhygbj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/goaeycnst.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gbxyzwuuv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/govhrmzfl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grdgcfuav.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjtucsmkp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/giobgxszy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gqaznfgqu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxnvltp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gsmzxsyta.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/grmtjozxv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdsdcmyjl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gnhwembsf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gmunibozv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gpzvtjknb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gpoajvfnu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gwcuftigy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvzmtkrgl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gmicbqrqe.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gifsuepqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gkddhpjjz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gegjzumkd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ggxpejchg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/guypmiuvf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gvtbbyivk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gchhqople.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gtanxpdwn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gnoxiyiep.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gynapbfkz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gfsxdsfty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/ghxqfqrlh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goefjhatj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gsivcichg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gnimqsqcl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqoutpisu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gvcugykyj.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ghxqwzxkr.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gnujviiox.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gczgcfhub.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gbsgfygwy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gjfotczxa.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gnvysxexu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/guegsyinl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gcslnlnhy.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/ggyqqjxwv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gqyfigxqh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcpemskoe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gltlnyfgn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwjhyvwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gxcjmcvuo.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gqsnekgqd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gcxglkbzv.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gcpjxgyvh.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gzaegjuhk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqcltzmoz.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gnriwhbin.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/ggvfmtjtn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gqwrqtbgc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gohrfoyem.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gmsqwywlm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gagccgboc.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gwsycpibm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gomeragpb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxncjov.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/glktikbcc.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gjtcnqyfu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gojgpscpu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gpvjbyjsi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gerjyfdqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/giryurgwm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gonmdhudo.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/ggnenmdem.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gkawfbuyv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gonjtpcoe.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gkgvkfwmi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gvhthtnwk.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkbvswhcq.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gesigjllz.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gbwjkwzvp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjnwawpsd.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gmlheryrj.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvxwshvel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/govekxvrn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gefubibbu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gbrudtgka.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbjdguxvb.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjoatzvwd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gpcpupwlu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/goxusenhg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gesycctfd.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gdgxzoxdw.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gxwvdkusl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gpgeyowdq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjclzdyls.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gogylkqef.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/geudiezvy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/glcifyipf.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gsgqvfzbd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gtvutymal.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gcsxasccs.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gnxjcnjus.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gbsrlywon.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/grpgwjcfh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/goektqjwc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gshnbziou.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gnxaxnktp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/giwupczuu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ghnbxgrhl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/ggdzbfjbx.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gjqvcvxlz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gblslqoko.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gjgjlhpne.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/ghgtxwhaa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gtvbligbj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gwvcynglw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gcdbvpvoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gnsqvicag.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gnkonwhvz.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gigxfynwk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgxkkwj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gyqmwuysb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gklosmsun.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmsmaqas.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gakborxwd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gvpbduegk.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcstyqaca.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gsxddvtrv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjgpkytxu.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gkwtlpmbs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/garbxtkbk.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfhurscwm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gkanzcial.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gzhzfnvne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gkstttmou.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/glxtaffqc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gqfkypcgp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/greyyenqe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gbeivsbjn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbrsmfkgs.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/glcijbsia.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjyblgqug.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gwoykykvr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdnjkcubb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gimkijbqo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/guvtxufkz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/goopzcgex.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gycvvtrdq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gbgadflat.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/goudmjdtk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gpmcatrwt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmbmlflfx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gdvrpktse.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grvmmqatg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyxlhgypb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/glpvejkuy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/ghybhppqo.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/golarbirn.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gfztsepli.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gkuqfxgxe.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gipbtcmhg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gvoznbxvr.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/goarialdw.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvszuvvpg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gmbdyakor.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkjlozcvt.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzouewvao.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gnnddwonc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/ghokuezfm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gtnjzjvhr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/ggttqvgrs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gayrwpalz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/guqenrqep.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gpymrkblc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gywncnlht.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/goyzkyhfu.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gaerlhxfo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwokmesck.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gcimhvqhj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdcylelvf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gspxwzsdb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjqwumuzb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/geutafhmy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxslgxorn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/guklkeeku.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gamvdmwyg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gpdepiomk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gryevyezu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/givoqbtzq.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gdffmququ.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gwiyczkqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gsjeuwfgo.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gipfbcqen.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gopckjnjg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gjimihdhn.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/goytkdvab.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gibxedmjm.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gotnpwfeh.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gicgqhmsj.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtknvhjh.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gpidhepgt.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grsmsblis.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gvvnztpjc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/getztdaep.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gwrcmgiap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqxstpbwq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsbwqjely.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnouvbzcj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gxvwhkafo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gmmggarri.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gpwhufens.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gimmulicn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/giuxgrggx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvckvunie.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gjyepymwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpuzyilsn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gwpolkqmw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ghqajshgd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/grwheravq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gglftbunp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/ghcihykbv.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gfpsbbjro.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gashyethm.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gkzpzuumr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gvoxusofw.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/geeinuqmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ghynfyqfr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gphpjqpec.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkevkxbwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gbbjwuqff.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gkwcqoyua.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gftqbnmbl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gwmzdrbja.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gionyvcdn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gtxirkjkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/golbviulo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gzycudxxm.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gleiufyfg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ghtfaxtlc.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gupbjhzws.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/ghzqsrhvb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gdrpwbvhr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpsyfxinj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gujprllrd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmickherc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gltgxxcvi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gukpexvsd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gzbthafzn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gipwlgoej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gsakwqpby.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gcltyvpgp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gnmflmvfg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ghnkaftic.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gixzyeizd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gyznlhyfd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gvepdcfkj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/giczctsnr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gtjemeobq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gcbdcfzrg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gnlhjxpxw.sHtML


<!-- 参考信息 -->